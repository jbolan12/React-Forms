# React-Forms

# Dynamic Greeting App

This React app allows users to input their name and receive a personalized greeting. The application demonstrates controlled inputs, form handling, and button hover effects for enhanced interactivity.

## Features

- **Dynamic Greeting**: Updates the greeting text based on user input.
- **Controlled Input Field**: The input is managed as state, ensuring real-time updates.
- **Button Hover Animation**: The submit button changes color when hovered, providing a smooth transition effect.

## Files

### `App.jsx`

- Contains the main `App` component where:
  - The `name` and `headingText` states manage the input and heading text respectively.
  - `handleChange` updates the `name` state as the user types.
  - `handleSubmit` sets the `headingText` with a greeting when the form is submitted, preventing page refresh.
  - Inline styles and hover events are applied to the submit button for a dynamic background and color change effect.

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/jbolan12/React-Forms.git
    ```
2. Navigate to the project directory:
    ```bash
    cd dynamic-greeting-app
    ```
3. Install the dependencies:
    ```bash
    npm install
    ```

## Usage

1. Start the development server:
    ```bash
    npm start
    ```
2. Open your browser and navigate to `http://localhost:3000` to view the app.

## Code Overview

- **State Management**:
  - `name` holds the input value, and `headingText` holds the greeting text displayed in the heading.
- **Controlled Input**:
  - The input field’s value is synced with `name`, allowing real-time updates and reset on submit.
- **Button Styling**:
  - Inline styles and `onMouseOver`/`onMouseOut` events animate the button on hover for a smooth effect.
 
## Dependencies
- React: 18.3.1
- React-DOM: 18.3.1
- React-Scripts 5.0.1


## License
This project is licensed under the MIT License. See the LICENSE file for details.

vbnet
Copiar código


### Code Example

```javascript
function handleSubmit(event) {
  setHeadingText(`Hello ${name}`);
  event.preventDefault();
}
