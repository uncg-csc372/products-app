# Full Stack React and Express Backend

This project is a full-stack application that combines a React frontend with an Express backend. It serves as a template for building web applications that require both client-side and server-side functionality.
## To Deploy to Render
1. Create a new Web Service on Render.
2. Connect your GitHub repository.
3. Specify the root directory to

```
react-client-express-backend/express-backend
```
in the build settings.
4. Set the build command to

```
npm install && npm run build
```
and the start command to

```node server.js
```
5. Add environment variable for your Neon database connection string

```DATABASE_URL
```with the value of your Neon database connection string.
6. Deploy the service and it should be live in a few minutes!