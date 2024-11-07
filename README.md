# bun-playground

playground for learning and practising bun

## Recommended Folder Structure

```md
my-bun-project/
├── src/
│ ├── server.ts # Main server entry point
│ ├── routes/
│ │ ├── index.ts # Define routes for the API
│ │ ├── userRoutes.ts # Example route file for user-related routes
│ │ └── ...
│ ├── controllers/
│ │ ├── userController.ts # Controllers handle the core business logic
│ │ └── ...
│ ├── middlewares/
│ │ ├── authMiddleware.ts # Authentication middleware
│ │ └── ...
│ ├── services/
│ │ ├── userService.ts # Service for user-related operations
│ │ └── ...
│ ├── utils/
│ │ ├── logger.ts # Utility for logging
│ │ └── constants.ts # Constants used throughout the app
│ └── ...
├── tests/
│ ├── server.test.ts # Example test file for the server
│ └── ...
├── public/ # Static assets (images, stylesheets, etc.)
│ ├── index.html # Main HTML file for static sites
│ └── ...
├── dist/ # Compiled files for production
├── package.json # Project dependencies and scripts
├── bun.lockb # Bun's lockfile (like package-lock.json)
├── README.md # Project documentation
└── tsconfig.json # TypeScript configuration
```

from inside your Bun project folder, here’s the command to create all the required folders and files in one line

```bash
mkdir -p src/{routes,controllers,middlewares,services,utils} tests public dist && \
touch src/{server.ts,routes/index.ts,routes/userRoutes.ts,controllers/userController.ts,middlewares/authMiddleware.ts,services/userService.ts,utils/{logger.ts,constants.ts}} tests/server.test.ts public/index.html package.json bun.lockb README.md tsconfig.json

```
