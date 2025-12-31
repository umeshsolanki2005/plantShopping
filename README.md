# Paradise Nursery - Plant Shopping Application

A modern, responsive React e-commerce application for browsing and purchasing plants. Built with React, Redux Toolkit, and Vite, featuring a complete shopping cart system with state management.

## 🌿 Features

- **Product Catalog**: Browse plants across multiple categories:
  - Air Purifying Plants
  - Aromatic Fragrant Plants
  - Insect Repellent Plants
  - Medicinal Plants
  - Low Maintenance Plants

- **Shopping Cart System**:
  - Add plants to cart with one click
  - Increment/decrement item quantities
  - Remove items from cart
  - Real-time total calculation
  - Cart item count badge in navbar

- **State Management**:
  - Global state management using Redux Toolkit
  - Persistent cart state across component navigation
  - Efficient reducer functions for cart operations

- **Responsive Design**:
  - Mobile-friendly layout
  - CSS Grid for product display
  - Flexbox navigation bar
  - Professional styling with custom CSS

## 🛠️ Tech Stack

- **Frontend**: React 18.2.0
- **State Management**: Redux Toolkit 2.2.3
- **Build Tool**: Vite 5.2.0
- **Styling**: CSS3
- **Deployment**: GitHub Pages
- **Package Manager**: npm

## 📦 Project Structure

```
src/
├── components/
│   ├── ProductList.jsx      # Product catalog and main page
│   ├── CartItem.jsx         # Shopping cart component
│   ├── AboutUs.jsx          # About page
│   └── App.jsx              # Main app component
├── slices/
│   └── CartSlice.jsx        # Redux slice for cart state
├── store.js                 # Redux store configuration
├── main.jsx                 # Application entry point
├── index.css                # Global styles
├── App.css                  # App component styles
├── ProductList.css          # Product listing styles
├── CartItem.css             # Cart component styles
└── AboutUs.css              # About page styles
```

## 🚀 Getting Started

### Prerequisites
- Node.js (v16 or higher)
- npm or yarn

### Installation

1. Clone the repository:
```bash
git clone https://github.com/umeshsolanki2005/plantShopping.git
cd plantShopping
```

2. Install dependencies:
```bash
npm install
```

3. Start the development server:
```bash
npm run dev
```

4. Open your browser and navigate to `http://localhost:5173`

## 📝 Available Scripts

- `npm run dev` - Start the development server
- `npm run build` - Build the project for production
- `npm run preview` - Preview the production build
- `npm run deploy` - Deploy to GitHub Pages
- `npm run lint` - Run ESLint to check code quality

## 🎯 Key Components

### ProductList Component
- Displays all plant products organized by category
- Implements the add-to-cart functionality
- Shows cart item count in navbar
- Handles cart visibility toggle

### CartItem Component
- Displays all items in the shopping cart
- Calculates individual item subtotals
- Calculates cart total amount
- Provides increment/decrement quantity controls
- Allows item removal from cart
- Continue shopping and checkout buttons

### CartSlice (Redux)
Manages cart state with three reducer functions:
- **addItem**: Adds a new plant or increments quantity if already in cart
- **removeItem**: Removes a plant from the cart
- **updateQuantity**: Updates the quantity of a specific plant

## 💳 Shopping Cart Functionality

### Adding Items to Cart
1. Browse products on the main page
2. Click "Add to Cart" button on any plant card
3. Button changes to "Added to Cart" when item is added
4. Cart count updates in the navbar

### Managing Cart Items
- **Increase Quantity**: Click the "+" button next to item quantity
- **Decrease Quantity**: Click the "-" button to decrease quantity
  - If quantity is 1, clicking "-" removes the item
- **Remove Item**: Click the "Delete" button to remove item from cart
- **Continue Shopping**: Return to product page while maintaining cart

### Price Calculation
- Individual item subtotal: Unit price × Quantity
- Total cart amount: Sum of all item subtotals
- All prices displayed in USD format

## 🌐 Live Demo

Visit the live application: [Paradise Nursery](https://umeshsolanki2005.github.io/plantShopping/)

## 🔧 Redux Architecture

### State Structure
```javascript
{
  cart: {
    items: [
      {
        name: string,
        image: string (URL),
        cost: string (e.g., "$15"),
        quantity: number
      }
    ]
  }
}
```

### Actions
- `addItem(product)` - Add product to cart
- `removeItem(productName)` - Remove product from cart
- `updateQuantity({ name, quantity })` - Update product quantity

## 🎨 Styling

The application features:
- Green color scheme for eco-friendly aesthetics
- CSS Grid layout for responsive product catalog
- Flexbox navbar for header alignment
- Hover effects on buttons and product cards
- Professional card-based design for products

## 📱 Responsive Features

- Mobile-optimized layout
- Touch-friendly buttons
- Responsive image sizing
- Flexible grid system that adapts to screen size

## 🚀 Deployment

The project is automatically deployed to GitHub Pages when code is pushed to the main branch. The deployment process:

1. Build the application: `npm run build`
2. Deploy to gh-pages: `gh-pages -d dist`
3. Live at: `https://umeshsolanki2005.github.io/plantShopping/`

## 📄 License

This project is open source and available under the MIT License.

## 👤 Author

Umesh Solanki

## 🤝 Contributing

Contributions are welcome! Feel free to:
1. Fork the repository
2. Create a feature branch (`git checkout -b feature/YourFeature`)
3. Commit your changes (`git commit -m 'Add YourFeature'`)
4. Push to the branch (`git push origin feature/YourFeature`)
5. Open a Pull Request

## 📞 Support

For questions or issues, please open an issue on the GitHub repository.

## 🎓 Learning Resources

This project demonstrates:
- React functional components and hooks (useState, useSelector, useDispatch)
- Redux Toolkit for state management
- Component composition and props
- Event handling in React
- Conditional rendering
- Array methods (map, filter, reduce)
- CSS Grid and Flexbox layouts
- GitHub Pages deployment

---

**Last Updated**: December 31, 2025
