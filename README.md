# Currency Converter App

This is a React-based Currency Converter application that allows users to convert currency amounts from one type to another using a third-party API for exchange rates.

## Table of Contents
- [Features](#features)
- [Components](#components)
  - [InputBox](#inputbox-component)
- [Custom Hooks](#custom-hooks)
  - [useCurrencyInfo](#usecurrencyinfo-hook)
- [Other Hooks](#other-hooks)
- [API](#api)
- [Getting Started](#getting-started)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Features
- Convert currency amounts from one type to another.
- Swap functionality to exchange the "from" and "to" currencies.
- Uses a third-party API to fetch the latest currency exchange rates.
- User-friendly UI with background image and responsive design.

## Components

### InputBox Component
The `InputBox` component is a reusable input field designed to handle both currency amount and type selection.

#### Props
- `label` (string): Label for the input box.
- `amount` (number): The current amount value.
- `onAmountChange` (function): Callback to handle amount changes.
- `onCurrencyChange` (function): Callback to handle currency type changes.
- `currencyOptions` (array): List of available currency options.
- `selectCurrency` (string): The currently selected currency type.
- `amountDisable` (boolean): Whether the amount input is disabled.
- `currencyDisable` (boolean): Whether the currency selection is disabled.
- `className` (string): Additional CSS classes for custom styling.

## Custom Hooks

### useCurrencyInfo Hook
The `useCurrencyInfo` hook fetches and returns the currency exchange rates for a given currency.

#### Parameters
- `currency` (string): The base currency to fetch exchange rates for.

#### Returns
- An object containing exchange rates of the base currency against other currencies.

## Other Hooks
- `useState`: Used to manage state within the component.
- `useEffect`: Used within the custom hook to fetch currency data when the currency changes.
- `useId`: Used in `InputBox` for generating unique IDs for input elements.

## API
This application uses the [currency-api](https://github.com/fawazahmed0/currency-api) to fetch the latest currency exchange rates. The API endpoint used in the custom hook is:
https://cdn.jsdelivr.net/npm/@fawazahmed0/currency-api@2024-03-06/v1/currencies/{currency}.json
Where `{currency}` is the base currency.

## Getting Started

### Prerequisites
- Node.js
- npm or yarn

### Installation
1. Clone the repository:
    ```
    git clone https://github.com/Vtsl-patel/currencyConverter.git
    ```
3. Navigate to the project directory:
    ```
    cd currencyConverter
    ```
4. Install the dependencies:
    ```
    npm install
    ```

## Usage
1. Start the development server:
    ```
    npm run dev
    ```
    
2. Open your browser and navigate to `http://localhost:3000` to see the app in action.

## Contributing
Contributions are welcome! Please open an issue or submit a pull request for any features, bug fixes, or enhancements.

---
Enjoy using the Currency Converter App! If you have any questions or need further assistance, feel free to reach out.

