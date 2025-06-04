# Spring GenAI Chat

This is a simple Spring Boot project that integrates with OpenAI's ChatGPT API using a RESTful interface. It also includes Swagger/OpenAPI documentation for easy testing and exploration.

## 🚀 Features

- Spring Boot 3.x
- Integration with OpenAI's GPT-3.5-turbo API
- REST endpoint to chat with the AI
- Swagger UI for testing the API

## 🧰 Prerequisites

- Java 17+
- Maven
- An OpenAI API key (get one from [https://platform.openai.com](https://platform.openai.com))

## 📦 How to Run

1. **Clone or unzip this project**

2. **Set your OpenAI API key**  
   Edit the file `src/main/resources/application.properties`:
   ```properties
   openai.api.key=sk-your_openai_api_key
   ```

3. **Build and run the app**:
   ```bash
   mvn spring-boot:run
   ```

4. **Test the endpoint using Swagger**:  
   Open your browser and go to:
   [http://localhost:8080/swagger-ui.html](http://localhost:8080/swagger-ui.html)

## 🛠 API Endpoint

### `POST /api/chat`

**Request Body**:
```json
{
  "message": "What is Spring Boot?"
}
```

**Response**:
```
"Spring Boot is a Java-based framework that simplifies building web apps..."
```

## 📁 Project Structure

```
spring-genai-chat/
├── pom.xml
├── README.md
└── src/
    └── main/
        ├── java/com/example/genai/
        │   ├── SpringGenAiChatApplication.java
        │   └── controller/ChatController.java
        └── resources/
            └── application.properties
```

## 🧪 Technologies Used

- Spring Boot
- OpenAI API
- Swagger (springdoc-openapi)
- RESTful Web Services

---

Made with ❤️ using Spring Boot and OpenAI