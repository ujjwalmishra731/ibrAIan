# 📚 LibrAIan

**LibrAIan** is your smart, AI-powered library assistant designed to help readers discover books by genre, mood, or author.  
Hosted Live 👉 [LibrAIan Web App](http://ujjwalmishra731.github.io/LibrAIan/)

---

## 🚀 Features

- 🔍 **Search bar** for books or authors
- 🎭 **Genre-based discovery** (Mystery, Romance, Sci-Fi, Non-fiction)
- 💬 **IBM Watson Chat Assistant** embedded for real-time conversation
- 🌐 **Responsive design** using Tailwind CSS
- ⚡ Fast, minimalist, and mobile-friendly

---

## 🧠 Tech Stack

- **HTML5** + **Tailwind CSS** for frontend
- **IBM Watson Assistant** for AI chatbot integration
- Hosted via **GitHub Pages**

---

## 🛠 How to Use

1. Visit the live site: [LibrAIan Web App](http://ujjwalmishra731.github.io/LibrAIan/)
2. Use the search bar to look up books or authors
3. Explore genres or start chatting with the AI bot for recommendations

---

## 💬 Chat Assistant Setup

This project integrates IBM Watson Assistant:

```js
<script>
  window.watsonAssistantChatOptions = {
    integrationID: "03423215-ca71-4ed0-80d8-aab48d199366",
    region: "eu-de",
    serviceInstanceID: "d6292216-9b26-4f79-825d-3bc1671f8c82",
    onLoad: async (instance) => { await instance.render(); }
  };
  setTimeout(function(){
    const t = document.createElement('script');
    t.src = "https://web-chat.global.assistant.watson.appdomain.cloud/versions/" + 
             (window.watsonAssistantChatOptions.clientVersion || 'latest') + "/WatsonAssistantChatEntry.js";
    document.head.appendChild(t);
  });
</script>

