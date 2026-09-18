# React + Spring Boot + MySQL demo

Небольшое учебное приложение, показывающее полный путь данных:

`React form -> fetch(JSON) -> Spring Boot REST API -> Spring Data JPA -> MySQL`

## Запуск

1. Запустите MySQL:

   ```bash
   docker compose up -d
   ```

2. В первом терминале запустите backend:

   ```bash
   cd backend
   mvn spring-boot:run
   ```

3. Во втором терминале установите зависимости и запустите React:

   ```bash
   cd frontend
   npm install
   npm run dev
   ```

4. Откройте <http://localhost:5173>.

Форма отправляет `POST /api/greetings`, а список загружается через `GET /api/greetings`.
