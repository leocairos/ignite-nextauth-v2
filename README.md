# NextAuth

How to create a next authentication and authorization app.

Requires:

  * Node 16+
  * yarn 1.22+
  

<br>

## How to create

<br> 

1. Create a next project

    ```shell
    yarn create next-app nextauth --ts
    ```

<br>

2. Edit /pages/_app.tsx

    ```javascript
    import {AppProps} from 'next/app'

    function MyApp({ Component, pageProps }: AppProps) {
      return <Component {...pageProps} />
    }

    export default MyApp
    ```
<br>

3. Edit/Create other files/folders

  * Create a context to auth
  * Implement login page on index.tsx
  * Create a api.ts on services folder
  * Create SSR global implementations on utils folder

<br>

## How to run

1. Run backend
   
    ```shel
    cd backend-api && yarn && yarn dev
    ```

<br>

2. Run frontend (in main folder)
   
    ```shel
    yarn && yarn dev
    ```