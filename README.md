<p align="center">
  <a href="http://nestjs.com/" target="blank"><img src="https://nestjs.com/img/logo_text.svg" width="320" alt="Nest Logo" /></a>
</p>

# Ejecutar en desarrollo

1. Clonar el repositorio.
2. Ejecutar:
```
yarn install
```
3. Instalar NestJs CLI:
```
npm i -g @nestjs/cli
```
4. Levantar la base de datos:
````
docker-compose up -d
````
5. Clonar el archvo __.env.template__ y renombrar a __.env__
6. Valores para trabajar en desarrollo:
````
MONGODB=mongodb://localhost:27017/nest-pokemon
PORT=3000
DEFAULT_LIMIT=5
````
7. Levantar el API:
````
yarn start:dev
````
8. Reconstruir la base de datos:
````
localhost:3000/api/v2/seed
````


##Stack
* NestJs
* MongoDB


#Notas
Heroku redeploy sin cambios:
````
git commit --allow-empty -m "Trigger Heroku deploy"
git push heroku main
`````
