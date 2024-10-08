# 🍕 Fast React Pizza Co.

This is a simple React application for a fictional pizza shop called "Fast React Pizza Co." It displays a menu of pizzas, each with ingredients, prices, and availability, and informs users about the shop's open hours.

## Features

- Displays a menu of available pizzas.
- Information about each pizza, such as ingredients, price, and whether it's sold out.
- Conditional rendering based on whether the shop is open.
- An order button appears when the shop is open.

- The app will be running at `http://localhost:3000`.

## Project Structure

- **index.js**: Entry point of the app, renders the main `App` component.
- **App.js**: The main application component that includes the header, menu, and footer.
- **Menu.js**: Displays a list of pizzas and handles the logic for showing the menu items.
- **Pizza.js**: Component to render individual pizza details (name, ingredients, price, sold-out status).
- **Footer.js**: Shows the shop's open hours and conditionally renders the order button based on the current time.

## Components

1. **`App`**

- The main component of the app. It includes three main sections: the Header, Menu, and Footer.

2. **`Header`**

- Displays the name of the pizza shop.

3. **`Menu`**

- Displays a list of pizzas by mapping over the pizza data.
- It conditionally renders the message if no pizzas are available.

4. **`Pizza`**

- Displays individual pizza details like name, ingredients, and price.
- Shows "SOLD OUT" if a pizza is not available.

5. **`Footer`**

- Checks the current time to see if the shop is open or closed and shows an order button if open.

6. **`Order`**

- Displays an order button and open hours.

## Data

The pizza menu is hardcoded in an array of objects in the component. Each object represents a pizza with the following properties:

- `name`: The name of the pizza.
- `ingredients`: A string listing the ingredients.
- `price`: Price of the pizza.
- `photoName`: A string with the path to the pizza image.
- `soldOut`: A boolean value indicating whether the pizza is sold out or not.
