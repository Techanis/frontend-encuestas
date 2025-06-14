# Pagina de proyecto "Encuestas"

Basado en [Guia de auth para Vue.js](https://developer.auth0.com/resources/guides/spa/vue/basic-authentication#add-user-logout-to-vue-js)


## Setear el proyecto

Crea un archivo .env y agrega las siguientes variables de prueba

VITE_API_SERVER_URL=http://localhost:6060
VITE_AUTH0_DOMAIN=dev-gvcplh7zbl6gqquj.us.auth0.com
VITE_AUTH0_CLIENT_ID=nu8W6SStnnTyBRHqU51uXx5DI47TQ9wo
VITE_AUTH0_CALLBACK_URL=http://localhost:4040/callback


Instala las dependencias

```bash
npm install
```

Inicia json server

```bash
npm run api
```

En otra terminal, inicia el dev server

```bash
npm run dev
```

Ingresa a  [`http://localhost:4040/`](http://localhost:4040/) para acceder a la aplicacion 

