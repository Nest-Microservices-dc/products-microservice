# product Microservice

## Dev

1. Clonar el repositorio
2. Instalar las dependencias `npm install && npm update`
3. Crear archivo `.env` basado en el `.env.example`
4. Ejecutar migracion de prisma `npx prisma migrate dev`
5. Levantar el servidor de NATS
```
docker run -d --name nats-main -p 4222:4222 -p 6222:6222 -p 8222:8222 nats
```
6. Levantar el servidor con `npm run start:dev`