# Stock Market Portfolio

A web application to manage and track your stock market investments. Built using the MERN (MongoDB, Express, React, Node.js) stack.

## Features

- User Authentication (Sign Up, Log In, Log Out)
- Add, update, and delete stock investments
- Real-time stock price updates
- Portfolio performance tracking
- Responsive design

## Demo

Check out the live demo [here](https://your-demo-link.com).

## Screenshots

![Home Page](screenshots/home.png)
![Portfolio Page](screenshots/portfolio.png)
![Stock Details Page](screenshots/stock-details.png)

## Installation

1. Clone the repository:

    ```bash
    git clone https://github.com/yourusername/stock-market-portfolio.git
    cd stock-market-portfolio
    ```

2. Install server dependencies:

    ```bash
    cd server
    npm install
    ```

3. Install client dependencies:

    ```bash
    cd ../client
    npm install
    ```

4. Set up environment variables:

    Create a `.env` file in the `server` directory with the following:

    ```env
    MONGO_URI=your_mongodb_connection_string
    JWT_SECRET=your_jwt_secret
    ALPHA_VANTAGE_API_KEY=your_alpha_vantage_api_key
    ```

5. Run the application:

    ```bash
    # Run server
    cd ../server
    npm start

    # Run client
    cd ../client
    npm start
    ```

    The server will start on `http://localhost:5000` and the client on `http://localhost:3000`.

## Technologies Used

- **MongoDB**: Database to store user and stock information
- **Express.js**: Backend framework
- **React**: Frontend library for building user interfaces
- **Node.js**: Runtime environment for server-side JavaScript
- **Axios**: For making API requests to fetch stock data
- **JWT**: For user authentication
- **Bootstrap**: For styling and responsive design

## Folder Structure

```
stock-market-portfolio/
├── client/
│ ├── public/
│ ├── src/
│ │ ├── components/
│ │ ├── pages/
│ │ ├── services/
│ │ ├── App.js
│ │ ├── index.js
│ │ └── ...
├── server/
│ ├── config/
│ ├── controllers/
│ ├── models/
│ ├── routes/
│ ├── server.js
│ └── ...
├── .gitignore
├── README.md
└── ...
```

## API Endpoints

### User Authentication

- `POST /api/auth/register`: Register a new user
- `POST /api/auth/login`: Log in a user
- `POST /api/auth/logout`: Log out a user

### Portfolio Management

- `GET /api/portfolio`: Get user's portfolio
- `POST /api/portfolio`: Add a new stock to the portfolio
- `PUT /api/portfolio/:id`: Update stock details
- `DELETE /api/portfolio/:id`: Delete a stock from the portfolio

### Stock Data

- `GET /api/stocks/:symbol`: Get stock details by symbol

## Contributing

Contributions are welcome! Please fork the repository and submit a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contact

For any inquiries, please contact me at [your-email@example.com].
