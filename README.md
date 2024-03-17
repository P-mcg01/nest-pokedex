<p align="center">
  <a href="http://nestjs.com/" target="blank"><img src="https://nestjs.com/img/logo-small.svg" width="200" alt="Nest Logo" /></a>
</p>

# Ejecutar en desarrollo

1. Clonar repositorio
2. Ejecutar

```properties
npm install
```

3. Tener Nest CLI instalado

```properties
npm i -g @nestjs/cli
```

4. Levantar la base de datos

```properties
docker compose up -d
```

5. Clonar el archivo **.env.template** y renombrar la copia a **.env**

6. Llenar las variables de entorno definidas en el **.env**

7. Ejecutar la aplicación en dev:

```properties
npm run dev
```

8. Reconstruir la base de datos con la semilla

```
http://localhost:3000/api/v2/seed
```

## Stack usado

- MongoDB
- Nest

## Production Build

1. Crear el archivo `.env.prod`
2. Llenar las variables de entorno
3. Crear la nueva imagen

```properties
docker compose -f docker-compose.prod.yaml --env-file .env.prod up --build
```
