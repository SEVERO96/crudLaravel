#Compilar y ejecutar el proyecto

### Ejecutar la base de datos de Postgres

Primero, necesitamos ejecutar la base de datos de Postgres.
  ```sh
	docker compose up -d db
  ```
Para verificar si se está ejecutando, puede usar el siguiente comando:
```sh
docker compose logs
  ```
y el

	```sh
	docker ps -a
	```
### Construye el proyecto

Para compilar el proyecto, escriba:
  ```sh
	docker compose build
  ```

###  Ejecutar el proyecto

PAhora podemos ejecutar el proyecto.
	```sh
docker compose up laravelapp
  ```

### Aplicar las migraciones

Para compilar el proyecto, escriba:
  ```sh
	docker compose exec laravelapp php artisan migrate
  ```

### Probar el proyecto
apis
- POST request to localhost:8000/api/players
- GET request to localhost:8000/api/players
- PUT request to localhost:8000/api/players/{id}
- GET request to localhost:8000/api/players/{id} (unjugador) 
- DELETE request to localhost:8000/api/players/{id}
