# Next JS SSR with Google OAuth

This is a simple example of how to implement Google OAuth in a Next.js application with server-side rendering (SSR). The example uses the `next-auth` library to handle authentication and session management.

## To Deploy to Render
1. Create a new Web Service on Render.
2. Connect your GitHub repository.
3. Specify the root directory to
```
nextjs-ssr-google-oauth
```
in the build settings.
4. Set the build command to
```
npm install && npm run build
```
and the start command to
```
npm start
```
5. Add environment variables for your Google OAuth credentials:
```
DATABASE_URL='NEON STRING'
clientID='clientIDFromGoogleCloud'
clientSecret='clientSecretFromGoogleCloud'
AUTH_SECRET='our_secret_key_for_next_auth-config'
```
6. Deploy the service and it should be live in a few minutes!
7. After the service is live, you need to register the origin and callback URL in your Google Cloud Console.
The origin should be in the format:
```
https://your-service.onrender.com
```

The callback URL should be in the format:
```
https://your-service.onrender.com/api/auth/callback/google
```

8. Once you have registered the origin and callback URL, you should be able to log in with Google on your deployed application!
