# AI Text Summarizing Application

## Application Objective

This application allows users to input text and generate AI-powered summaries. The user can:

1. Enter or paste text in a textarea.
2. Submit the text using a “summarize” button.
3. Receive an AI-generated summary in an output textarea.

---

## Application Structure

![Application Structure](https://prod-files-secure.s3.us-west-2.amazonaws.com/1facb56d-497f-48ac-827b-24d0c0b8d250/cd6b4212-7a1b-4c77-81b7-bcd54a697691/image.png)

- **package.json**: Contains metadata about the app and the packages used for development and production.
  
### Server
- **index.js**: Starts the [Express](https://expressjs.com/en/starter/hello-world.html) server.
- **summarize.js**: Contains a function to make requests to the Hugging Face Inference API for text summarization.

### Client
- **public folder**: Contains the frontend code.
  - **index.html**: Structure of the webpage.
  - **stylesheet.css**: Styling for the webpage.
  - **script.js**: Handles user interactions, such as submitting text and receiving a summary.

---

## Steps and Requirements

1. **Set up a [Replit](https://docs.replit.com/programming-ide/introduction-to-the-workspace) account** for deployment.
2. **Create a [Hugging Face](https://huggingface.co) account** for API access.
3. **Install [Postman](https://www.postman.com/)** for API testing.
4. **Set up [Express.js](https://expressjs.com/en/starter/installing.html)** using npm for server-side code.
5. Use basic **HTML, CSS, and JavaScript** for the frontend.

---

## Key User Interactions

### In the frontend (JavaScript):
1. **Text Input**: Allow users to type or paste text into a `textarea` and ensure it complies with character limits.
2. **Submit Button**: Users can click the “Summarize” button to generate a summary.

### In the backend (Express):
1. Add a **`/summarize` endpoint** that accepts POST requests from the frontend.
2. Create a function that calls the **Hugging Face Inference API** to generate a summary using **Facebook’s "bart-large-cnn" model**.
3. Use **Postman's code generation feature** and the **axios** library for making HTTP requests.

---

## Functions

### Frontend Functions:
- **`verifyTextLength`**: Validates the text length to ensure it's within the allowed limits.
- **`submitData`**: Handles the submission of text for summarization.

### Backend Functions:
- **Summarize Function**: Calls the Hugging Face Inference API to generate the summary. This function is used in the `/summarize` endpoint.

---

## Tech Stack

### API Platform
- [Postman](https://www.postman.com/)

### Code Editor / Deployment Tool
- [Replit](https://docs.replit.com/programming-ide/introduction-to-the-workspace)

### Backend
- [Node.js](https://nodejs.org/en/docs)
- [Express](https://expressjs.com/en/starter/hello-world.html)
- [Hugging Face Inference API](https://huggingface.co/docs/api-inference/index)

### Frontend
- HTML
- CSS
- JavaScript

---

This `README.md` file provides a detailed explanation of the project and contributed by @Brijeshhhh
