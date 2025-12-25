
## Test React and Node.Js with Multi-Stage

Frontend - React
Backend - Node.js (API)
Multi-Stage Dockerfile

--

Build and Run Backend

```
docker build -t react-backend .
docker run -d -p 3000:3000 react-backend
```

Testing

http://localhost:3000/api

{ "message": "Hello, I'm Backend API" }


--

Build and Run Frontend

```
docker build -t react-frontend .
docker run -d -p 8080:80 react-frontend
```

Testing

React UI - http://localhost:8080
Backend API - http://localhost:3000/api
