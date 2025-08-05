# Point Tils TESTE

## 🚀 Tecnologias

- **[React Native](https://reactnative.dev/)** - Framework para desenvolvimento mobile
- **[Expo](https://expo.dev/)** - Plataforma para desenvolvimento universal
- **[TypeScript](https://www.typescriptlang.com/)** - Linguagem de programação
- **[EAS](https://docs.expo.dev/eas/)** - Expo Application Services para build e deploy

## 📦 Pré-requisitos

Antes de começar, você precisa ter instalado:

- **Node.js** (versão 18 ou superior)
- **npm** ou **yarn**
- **Expo CLI**: `npm install -g @expo/cli`
- **EAS CLI**: `npm install -g eas-cli`
- **Git**

### Para desenvolvimento:
- **Expo Go** (para emulador Android ou iOS)
- **Xcode** (para simulador iOS - apenas macOS)

## 🛠️ Desenvolvimento

1. **Instale as dependências**
   ```bash
   cd point-tils
   npm install
   ```

2. **Configure o EAS**
   ```bash
   eas login
   eas build:configure
   ```

### 🔧 Desenvolvimento Local

| Comando | Descrição |
|---------|-----------|
| `npm start` | Inicia o servidor de desenvolvimento |
| `npm run lint` | Executa verificação de código (ESLint) |

> #### Testando
>
> - **Android**: Expo Go
> - **iOS**: Expo Go ou Simulador XCode

### 🏗️ Build (Geração de artefatos)

| Comando | Plataforma | Descrição |
|---------|------------|-----------|
| `npm run build:dev` | Android + iOS | Build desenvolvimento para ambas plataformas |
| `npm run build:preview` | Android + iOS | Build preview/teste para ambas plataformas |
| `npm run build:android` | Android | Build apenas para Android (APK) |
| `npm run build:ios` | iOS | Build apenas para iOS (IPA) |

> #### Artifacts Gerados
>
> - **Android**: Arquivo `.apk` para instalação direta
> - **iOS**: Arquivo `.ipa` para distribuição via TestFlight/App Storen

## 💰 **Custos**

| Ação | iOS | Android |
|------|-----|---------|
| **Expo Go (desenvolvimento)** | ✅ Gratuito | ✅ Gratuito |
| **Build** (gerar IPA/APK) | ❌ $99/ano | ✅ Gratuito |
| **Deploy** (TestFlight/App Store) | ❌ $99/ano | ✅ Gratuito ($25 Play Store) |

> **⚠️ Importante:** Para iOS, até builds de development precisam de Apple Developer Account