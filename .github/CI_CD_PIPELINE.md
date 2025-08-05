# CI/CD Pipeline Documentation

## Pipeline de Build e Checks para PRs

Este repositório implementa um pipeline robusto de CI/CD para garantir a qualidade do código em Pull Requests.

## 🔍 Checks Executados em PRs

### 1. **PR Agent Review**

- 🤖 Revisão automática de código com IA
- 📝 Geração automática de descrição do PR
- 💡 Sugestões de melhorias no código
- ⏱️ ~1-2 minutos

### 2. **Lint and Type Check**

- ✅ ESLint para verificar padrões de código
- ✅ TypeScript type checking
- ⏱️ ~2-3 minutos

### 3. **Code Formatting Check**

- ✅ Prettier para verificar formatação consistente do código
- ✅ Padronização de estilo de código
- ⏱️ ~1-2 minutos

### 4. **Build Check**

- ✅ Prebuild para Android e iOS
- ✅ Verificação se o projeto compila corretamente
- ⏱️ ~5-8 minutos

### 5. **Dependency Analysis**

- ✅ Análise de dependências não utilizadas
- ✅ Verificação do tamanho do bundle
- ⏱️ ~2-3 minutos

### 6. **Security Audit**

- ✅ npm audit para vulnerabilidades conhecidas
- ✅ Verificação de dependências inseguras
- ⏱️ ~1-2 minutos

### 7. **Expo Doctor**

- ✅ Verificação de configuração do Expo
- ✅ Detecção de problemas de compatibilidade
- ⏱️ ~1-2 minutos

## 🤖 PR Agent Features

### Revisão Automática:

- Análise de qualidade do código
- Detecção de possíveis bugs
- Verificação de boas práticas
- Sugestões de otimização

### Descrição Automática:

- Geração de descrição baseada nas mudanças
- Listagem de funcionalidades adicionadas
- Documentação automática de breaking changes

## 🌙 Nightly Build

### Workflow Automático:

- ⏰ Executa todo dia às 3h UTC
- 🔍 Verifica vulnerabilidades de segurança
- 📈 Gera relatórios de dependências desatualizadas
- 🔄 Atualiza automaticamente dependências patch/minor
- 📊 Monitora a saúde geral do projeto

### Benefícios:

- Detecção precoce de problemas de segurança
- Manutenção automática de dependências
- Prevenção de acúmulo de dívida técnica

## 🛡️ Proteção de Branches

### Branch `main`:

- ✅ Obrigatório aprovação de 1 reviewer
- ✅ Obrigatório code owner approval (@Bialves)
- ✅ Todos os checks devem passar
- ✅ Branch deve estar atualizada antes do merge

## 🚨 Resolução de Problemas

### Falha no Lint:

```bash
npm run lint:fix
```

### Falha na Formatação:

```bash
npm run format
```

### Falha no Type Check:

```bash
npm run type-check
```

### Falha no Build:

```bash
npm run doctor
npm run prebuild:clean
```

### PR Agent Issues:

- O PR Agent roda apenas em pull requests
- Falhas não bloqueiam o merge (apenas informativos)

## 📚 Recursos Adicionais

- [Expo Documentation](https://docs.expo.dev/)
- [React Native Testing Library](https://callstack.github.io/react-native-testing-library/)
- [ESLint Expo Config](https://docs.expo.dev/guides/using-eslint/)
- [GitHub Actions](https://docs.github.com/en/actions)
- [PR Agent Documentation](https://github.com/Codium-ai/pr-agent)
