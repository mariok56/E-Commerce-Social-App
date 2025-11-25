React Native Assignment: E‑Commerce & Social App

A full‑featured mobile application built with React Native and TypeScript. This project showcases clean architecture, modern state management, API integration, theming and responsive UI. It includes authentication flows, product management (list, add, edit, details), a simple posts feed, profile editing and a dark/light theme toggle.

⭐ Features

Authentication – Register, Login, Email verification and Forgot Password flows with form validation (react-hook-form + zod) and API integration.

User Profile – Upload a profile picture (camera & gallery support), view and edit profile information.

Product Catalog

Infinite scrolling product list with search, filters and sort (price or creation date).

Product details view with rich information.

Add and edit products (forms with validation).

Dark/light theme support on every screen.

Posts Feed – Simple social posts tab (placeholder for blog/news feed).

State Management – Uses React Context & Zustand store for authentication state, plus TanStack React Query
 for data fetching, caching and pagination.

Navigation – Stack and bottom tab navigators via @react-navigation/native and @react-navigation/bottom-tabs.

API Integration – Axios instance with token storage and authentication via secure storage (see src/lib/axioInstance.ts).

Theming & Responsiveness – Custom ThemeContext, dark/light mode toggle, and responsive helper utilities.

Atomic Design – Components organised into atoms, molecules and organisms for scalability and readability.

🛠 Tech Stack

React Native CLI with TypeScript

React Navigation for stack & tab navigation

React Hook Form & Zod for forms and validation

TanStack React Query for server state management

Axios for API calls

Zustand for client state (auth store)

react-native-safe-area-context for SafeArea support

react-native-image-picker for camera/gallery access

Tailwind‑like helper functions in utils/responsive.ts for consistent sizing

Dark/Light theme context with custom colours

📲 Screenshots

Add screenshots or screen recordings of key flows here (Authentication, Product List & Details, Add/Edit Product, Posts, Profile). Visuals help reviewers understand the UX quickly.

📂 Project Structure
src/
├── components/        # atomic design components (atoms, molecules, organisms)
├── contexts/          # ThemeContext and other providers
├── hooks/             # Custom hooks (useAuth, useProducts, etc.)
├── lib/               # API client and helper libraries
├── navigation/        # Stack & Tab navigators
├── screens/           # Screen components grouped by feature
├── services/          # API service functions
├── store/             # Zustand stores (auth)
├── types/             # Shared TypeScript types
└── utils/             # Helpers (responsive sizes, fonts, validation schemas)

🚀 Getting Started
Prerequisites

Node.js >= 16 and npm or Yarn

React Native development environment (Android Studio / Xcode) set up. Follow the React Native docs
 for detailed instructions.

Installation

Clone the repository

git clone https://github.com/mariok56/React_Native_Assignment.git
cd React_Native_Assignment


Install dependencies

# using npm
npm install

# or using Yarn
yarn install


Start the Metro bundler

# npm
npm start
# or yarn
yarn start


Run on Android

npm run android
# or
yarn android


Run on iOS

# install CocoaPods dependencies (only on first run or after native deps change)
bundle install
bundle exec pod install

npm run ios
# or
yarn ios


Configure API

The app expects a backend API for authentication, products and posts. Update the base URL and endpoints in src/lib/axioInstance.ts and src/services/* to point to your server. For secure authentication, tokens are stored using @react-native-async-storage/async-storage (see src/lib/axioInstance.ts).

🧪 Testing & Linting

This repo does not include unit tests yet. Consider adding tests with Jest and React Native Testing Library.

Run eslint and prettier to ensure code quality.

npm run lint    # check for lint errors
npm run format  # format code with Prettier

🤝 Contributing

Contributions are welcome! Feel free to open issues or submit pull requests. For major changes, please open an issue first to discuss what you would like to change.

📄 License

This project is released under the MIT License
. You are free to use, modify and distribute it as long as you include the original license text.

👤 Author

Mario Karam
 – Frontend & Mobile Developer. If you have any questions, please reach out via LinkedIn
 or email.
