# Project Overview

This project, **Point Tils**, is a mobile application built with React Native and Expo. It supports Android and iOS, and includes features such as theming, animations, and file-based routing.

## Folder Structure

- `/app`: Contains the main application code, including screens and layouts.
- `/components`: Reusable UI components.
- `/hooks`: Custom React hooks for shared logic, including utilities for theming and color schemes.
- `/constants`: Shared constants such as colors and configurations.
- `/assets`: Static assets like images and fonts.
- `/app.json`: Expo configuration file.
- `/eas.json`: Configuration for Expo Application Services (EAS).

## Libraries and Frameworks

- **React Native**: Core framework for mobile development.
- **Expo**: Platform for universal app development.
- **TypeScript**: For type safety and better developer experience.
- **React Navigation**: For navigation and routing.
- **React Native Reanimated**: For animations.
- **Expo Router**: For file-based routing.
- **ESLint**: For linting and code quality.
- **Prettier**: For consistent code formatting.

## Coding Standards

- Use **English** for all code, comments, and documentation.
- Avoid verbose comments; only include comments when necessary to clarify complex logic.
- Follow TypeScript strict mode for type safety.
- Use single quotes for strings.
- Use arrow functions for callbacks and functional components.
- Maintain consistent formatting with Prettier and ESLint.
- Avoid unused imports and dependencies.

## UI Guidelines

- Follow light and dark mode theming using the `useThemeColor` hook.
- Ensure components are reusable and follow a modular design.
- Use animations sparingly and only when they enhance the user experience.

## Additional Notes

- Follow the folder structure and naming conventions for new files and components.
- Use the `Colors` constant for consistent theming.
- Avoid hardcoding styles; use shared constants or stylesheets.
- Ensure compatibility with Android and iOS.
- Use Expo's `expo-router` for navigation and routing.
