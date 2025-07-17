# AIConstructor
# Coding Instructor AI (with Gemini-1.5-flash)

This project integrates the **Google Gemini AI** model to create a **Coding Instructor AI** that helps users with **Data Structures and Algorithms** (DSA) related queries. It answers DSA questions **politely** and **rudely dismisses unrelated questions** (intentionally) — as a quirky feature for educational humor or testing.

## 💡 Features

* Uses **Google Gemini 1.5 Flash** model via `@google/genai`.
* Provides **clear and concise** explanations for DSA questions.
* Responds **rudely and humorously** to off-topic or non-DSA queries.
* Demonstrates basic frontend usage with JavaScript and HTML.

## 🚀 Getting Started

### 1. Install dependencies

```bash
npm install @google/genai
```

### 2. Set up your API key

Replace the placeholder API key in the code:

```javascript
const ai = new GoogleGenAI({
  apiKey: "AIzaSyCBgwqxosP7qA-RCEjkeZHIXmh-APYYCLk" 
});
```

> ⚠️ Never expose API keys in production. Use environment variables or secure vaults.

### 3. Run the App

If you are using Node.js:

```bash
node index.js
```

Or open the `index.html` in your browser to see the sample interaction in action.

## 📁 Project Structure

```
coding-instructor-ai/
│
├── index.html        # Frontend interaction sample
├── index.js          # Main Node.js logic using Gemini AI
├── README.md         # Project documentation
```

## 🧠 Example Behavior

### ✅ DSA Question

> ❓ What is a closure in JavaScript?
> ✅ Response: \[Polite explanation about closures with example]

### ❌ Non-DSA Question

> ❓ Who is the president of the USA?
> ❌ Response: "You dumb, ask me some sensible question related to DSA."

## 🧬 Why So Rude?

This behavior is controlled using the `systemInstruction` in the Gemini AI prompt configuration. It's a fun and educational constraint to explore prompt engineering and AI model behaviors.

## 📜 License

MIT License

---

**Note**: This is a demo project. The rude response behavior is for **educational and experimental purposes** only and not intended for actual user-facing systems.

