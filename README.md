# Quickish

![logo-quickish](https://github.com/user-attachments/assets/0cad52c3-4de8-4c9d-b524-2bfafb5b8020)

Quickish es una aplicación de pedidos de comida a domicilio en proceso de desarrollo. Permite a los Clientes explorar restaurantes y gestionar pedidos; a los Restaurantes, administrar su catálogo y procesar pedidos; al Repartidor transportar pedidos desde el Restaurante a la dirección del Cliente y al Administrador, supervisar usuarios.
___

## Equipo de trabajo
- [Felipe Alvarez](https://github.com/felialvarez)
- [Tomas Jopia](https://github.com/jopiatomas)
- [Lucas Monti](https://github.com/Lucasmonti)
- [Bruno Logghe](https://github.com/brunologghe)
___

# Requisitos previos
Antes de correr el proyecto, asegurate de tener instalados globalmente:
- [Node.js](https://nodejs.org/) (Se recomienda v22+)
- [Angular CLI](https://angular.io/cli)
- [json-server](https://www.npmjs.com/package/json-server)
- [Java JDK](https://adoptium.net/) (Se recomienda JDK 17+)
- [MySQL](https://www.mysql.com/downloads/)

Instala Angular CLI y json-server de la siguiente manera:
```bash
npm install -g @angular/cli json-server
```
___

# Pasos para hacer funcionar la aplicación

1. **Instala las dependencias del frontend:**
   ```bash
   npm install
   ```
2. **Navega hasta la carpeta del proyecto frontend:**
   ```bash
   cd code
   ```
3. **Corre el proyecto frontend:**
   ```bash
   ng serve -o
   ```
4. **Configura y ejecuta el backend** (necesario para el funcionamiento completo del sistema):

   - **Clona el repositorio del backend:**
     ```bash
     git clone https://github.com/felialvarez/quickish.git 
     cd quickish
     ```
   - **Backend (Spring Boot)**
     ```bash
     cd backend 
     ./mvnw spring-boot:run
     ```
     El backend se ejecuta en:
     ```bash
     http://localhost:8080
     ```
   - **Frontend (Angular)**
     ```bash
     cd frontend
     npm install 
     npm start
     ```
     El frontend se ejecuta en:
     ```bash
     http://localhost:4200
     ```
     > **Importante:** Asegúrate de tener Java JDK instalado y las extensiones de Java configuradas en Visual Studio Code.  
     > Además, el backend debe estar corriendo antes de utilizar la aplicación frontend para que el sistema funcione correctamente.
     
   - **Configura la conexión a la base de datos MySQL:**
     - Crea una base de datos nueva en MySQL (por ejemplo, `quickish_db`).
     - Abre el archivo `src/main/resources/application.properties` en el backend.
     - Modifica las siguientes líneas con los datos de tu base de datos local:
       ```
       spring.datasource.url=jdbc:mysql://localhost:3306/quickish_db
       spring.datasource.username=TU_USUARIO
       spring.datasource.password=TU_PASSWORD
       ```

5. **¡Listo! Ya podés utilizar Quickish sin problemas.**
___

# Tecnologías utilizadas

- **Frontend:** Angular
- **Backend:** Spring Boot (Java)
- **Base de datos:** MySQL

---
