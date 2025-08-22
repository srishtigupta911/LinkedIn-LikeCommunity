# LinkedIn Community Platform - Frontend

This is the React frontend for the LinkedIn Community Platform, a full-featured social networking application built with modern web technologies.

## Overview

The frontend is built with React 19 and Material-UI, providing a beautiful and responsive user interface for the LinkedIn Community Platform. It includes advanced features like real-time search, image uploads, and a comprehensive follow system.

## Features

### Core Functionality
- **User Authentication**: Secure login and registration with JWT tokens
- **Post Management**: Create, view, and delete posts with text and images
- **User Search**: Real-time search functionality with debounced input
- **Follow System**: Follow/unfollow other users to build your network
- **Profile Management**: View and edit user profiles

### UI/UX Features
- **Responsive Design**: Works seamlessly on desktop, tablet, and mobile
- **Material-UI Components**: Professional and modern interface
- **Real-time Updates**: Posts and interactions update automatically
- **Loading States**: Smooth loading indicators throughout the app
- **Error Handling**: Comprehensive error handling and user feedback

### Technical Features
- **React 19.1.1**: Latest React with modern hooks and features
- **React Router 7.7.1**: Client-side routing with protected routes
- **Material-UI 7.3.0**: Professional UI component library
- **Axios**: HTTP client for API communication
- **Context API**: Global state management for authentication

## Project Structure

```
frontend/
├── public/                 # Static assets
│   ├── index.html         # Main HTML file
│   ├── favicon.ico        # App icon
│   └── manifest.json      # PWA manifest
├── src/
│   ├── components/        # Reusable components
│   │   ├── Header.js      # Navigation header with search
│   │   ├── PostCard.js    # Individual post display
│   │   ├── PostForm.js    # Post creation form
│   │   ├── SearchBar.js   # User search functionality
│   │   ├── Loader.js      # Loading component
│   │   └── PrivateRoute.js # Protected route wrapper
│   ├── contexts/          # React contexts
│   │   └── AuthContext.js # Authentication context
│   ├── pages/             # Page components
│   │   ├── Home.js        # Main feed page
│   │   ├── Login.js       # Login page
│   │   ├── Register.js    # Registration page
│   │   └── Profile.js     # User profile page
│   ├── services/          # API services
│   │   └── api.js         # API communication layer
│   ├── App.js             # Main app component
│   ├── App.css            # App styles
│   └── index.js           # App entry point
└── package.json           # Dependencies and scripts
```

## Available Scripts

### `npm start`

Runs the app in development mode.\
Open [http://localhost:3000](http://localhost:3000) to view it in your browser.

The page will reload when you make changes.\
You may also see any lint errors in the console.

### `npm test`

Launches the test runner in interactive watch mode.\
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

### `npm run build`

Builds the app for production to the `build` folder.\
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.\
Your app is ready to be deployed!

### `npm run eject`

**Note: this is a one-way operation. Once you `eject`, you can't go back!**

If you aren't satisfied with the build tool and configuration choices, you can `eject` at any time. This command will remove the single build dependency from your project.

Instead, it will copy all the configuration files and the transitive dependencies (webpack, Babel, ESLint, etc) right into your project so you have full control over them. All of the commands except `eject` will still work, but they will point to the copied scripts so you can tweak them. At this point you're on your own.

You don't have to ever use `eject`. The curated feature set is suitable for small and middle deployments, and you shouldn't feel obligated to use this feature. However we understand that this tool wouldn't be useful if you couldn't customize it when you are ready for it.

## Key Components

### Header Component
- Navigation bar with logo and user menu
- Integrated search bar for finding users
- Responsive design with mobile menu
- User authentication status display

### PostCard Component
- Displays individual posts with user information
- Shows post content and uploaded images
- Delete functionality for post authors
- Responsive image gallery

### PostForm Component
- Rich text input for post creation
- Multiple image upload support (up to 5 images)
- File type validation (JPEG, PNG, GIF)
- Real-time character count and validation

### SearchBar Component
- Real-time user search with debounced input
- Search results with user avatars
- Click-to-navigate functionality
- Loading states and error handling

## Environment Variables

Create a `.env` file in the frontend directory:

```env
REACT_APP_API_URL=http://localhost:5000
```

For production, set this to your backend service URL.

## Dependencies

### Core Dependencies
- **react**: ^19.1.1 - React library
- **react-dom**: ^19.1.1 - React DOM rendering
- **react-router-dom**: ^7.7.1 - Client-side routing
- **@mui/material**: ^7.3.0 - Material-UI components
- **@mui/icons-material**: ^7.3.0 - Material-UI icons
- **@emotion/react**: ^11.14.0 - CSS-in-JS styling
- **@emotion/styled**: ^11.14.1 - Styled components
- **axios**: ^1.11.0 - HTTP client

### Development Dependencies
- **react-scripts**: 5.0.1 - Create React App scripts
- **@testing-library/react**: ^16.3.0 - React testing utilities
- **@testing-library/jest-dom**: ^6.6.4 - Jest DOM matchers
- **@testing-library/user-event**: ^13.5.0 - User event simulation

## Browser Support

This app supports all modern browsers:
- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)

## Performance Optimizations

- **Code Splitting**: Automatic code splitting with React Router
- **Image Optimization**: Automatic image compression and lazy loading
- **Bundle Optimization**: Minified production builds
- **Caching**: Efficient caching strategies for static assets

## Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## Learn More

You can learn more in the [Create React App documentation](https://facebook.github.io/create-react-app/docs/getting-started).

To learn React, check out the [React documentation](https://reactjs.org/).

---



This frontend was developed as part of the LinkedIn Community Platform, demonstrating modern React development practices with Material-UI and comprehensive social networking features.
