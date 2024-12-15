# Airbnb Clone

A full-stack Airbnb clone that replicates the core functionalities of the Airbnb platform. This project includes user authentication, property listings, search filters, booking functionality, and a responsive user interface.

## Features

- **User Authentication**: Sign up, log in, and manage profiles.
- **Property Listings**: Users can list properties, including photos, descriptions, and pricing.
- **Search and Filters**: Search for properties by location, price range, and more.
- **Booking System**: Book properties with a built-in calendar and availability tracking.
- **Responsive Design**: Optimized for desktop, tablet, and mobile devices.
- **Payment Integration**: Simulated payment system (Stripe integration).

---

## Tech Stack

- **Frontend**: React.js, Redux, TailwindCSS, Bootstrap
- **Backend**: Node.js, Express.js
- **Database**: MongoDB
- **Authentication**: JWT (JSON Web Tokens), bcrypt
- **Payments**: Stripe API for payment simulation
- **Cloud Storage**: AWS S3 for property image uploads

---

## Installation and Setup

Follow these steps to get the Airbnb clone running locally on your system:

### Prerequisites

1. **Node.js**: Download and install [Node.js](https://nodejs.org/).
2. **MongoDB**: Set up a local or cloud MongoDB instance.
3. **Stripe Account**: Create a [Stripe account](https://stripe.com) to get API keys.
4. **AWS S3**: Set up an AWS S3 bucket for storing property images.

### Clone the Repository

```bash
git clone https://github.com/pawarchandrakant29/airbnb-clone.git
cd airbnb-clone
```

### Backend Setup

1. Navigate to the `server` folder:
   ```bash
   cd backend
   ```
2. Install dependencies:
   ```bash
   npm install
   ```
3. Create a `.env` file in the `server` folder and configure the following:
   ```env
   JWT_SECRET=your_jwt_secret_key
   JWT_EXPIRY=20d
   VITE_GOOGLE_CLIENT_ID=your_ID
   COOKIE_TIME=7
   SESSION_SECERET=secret_key
   CLOUDINARY_NAME=your_name
   CLOUDINARY_API_KEY=KEY
   CLOUDINARY_API_SECERET=SECRET_KEY
   CLIENT_URL=YOUR URL
   ```
4. Start the backend server:
   ```bash
   npm start
   ```
   The backend server will start on `http://localhost:3000`.

### Frontend Setup

1. Navigate to the `client` folder:
   ```bash
   cd ../client
   ```
2. Install dependencies:
   ```bash
   npm install
   ```
3. Create a `.env` file in the `frontend` folder and add the backend API base URL:
   ```env
   REACT_APP_API_URL=http://localhost:3000
   REACT_APP_STRIPE_PUBLIC_KEY=your_stripe_public_key
   ```
4. Start the frontend server:
   ```bash
   npm start
   ```
   The frontend server will start on `http://localhost:5173`.

---

## Usage

1. Open `http://localhost:5173` in your browser.
2. Sign up or log in to your account.
3. Browse available properties and use search filters to refine your results.
4. Book a property, upload new listings, or manage existing listings.
5. Simulate payments using the Stripe integration.

---

## Acknowledgements

- [Airbnb](https://www.airbnb.com) for the inspiration.
- [Stripe API](https://stripe.com/docs/api) for payment integration.
- [AWS S3](https://aws.amazon.com/s3/) for cloud storage.
- Open-source libraries and tools used in this project.

