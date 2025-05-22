# Frontend Application (Next.js)

This is the frontend application built with Next.js, TypeScript, and Tailwind CSS.

## Development

### Prerequisites
- Node.js (version 18.x or higher recommended)
- npm

### Installing Dependencies
To install the necessary dependencies, navigate to the `frontend` directory and run:
```bash
npm install
```

### Running the Development Server
To start the development server, run:
```bash
npm run dev
```
The application will be accessible at [http://localhost:3000](http://localhost:3000). The page auto-updates as you edit the files.

### Building the Application
To build the application for production, run:
```bash
npm run build
```
This will create an optimized build in the `.next` directory.

### Starting the Production Server
After building the application, you can start the production server by running:
```bash
npm run start
```
This will serve the application from the `.next` folder, typically on port 3000.

## Docker
This application can also be built and run using Docker. Refer to the main `README.md` in the root directory for instructions on using Docker Compose.
