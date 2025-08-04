# 📚 LibrAIan

**LibrAIan** is your AI-powered library assistant designed to help users discover books based on genres, moods, and authors. With a sleek, modern interface and Watson Assistant integration, LibrAIan makes book discovery interactive and intelligent.

🌐 **Live Site**: [ujjwalmishra731.github.io/LibrAIan](http://ujjwalmishra731.github.io/LibrAIan/)

---

## 🚀 Features

- 🔍 Search bar for books or authors
- 🎯 Genre-based discovery (e.g., Mystery, Romance, Sci-Fi, Non-fiction)
- 🤖 IBM Watson Chat Assistant for interactive book recommendations
- 🌈 Responsive design built with Tailwind CSS
- ⚡ Fast, lightweight, and user-friendly interface

---

## 🧠 Technologies Used

- **HTML5**
- **Tailwind CSS**
- **JavaScript (for Watson integration)**
- **IBM Watson Assistant**
- **GitHub Pages** for deployment

---

## 💬 IBM Watson Assistant Integration

The chatbot is embedded using the following script inside the HTML:

```html
<script>
  window.watsonAssistantChatOptions = {
    integrationID: "03423215-ca71-4ed0-80d8-aab48d199366", // The ID of this integration.
    region: "eu-de", // The region your integration is hosted in.
    serviceInstanceID: "d6292216-9b26-4f79-825d-3bc1671f8c82", // The ID of your service instance.
    onLoad: async (instance) => { await instance.render(); }
  };
  setTimeout(function(){
    const t = document.createElement('script');
    t.src = "https://web-chat.global.assistant.watson.appdomain.cloud/versions/" + 
             (window.watsonAssistantChatOptions.clientVersion || 'latest') + "/WatsonAssistantChatEntry.js";
    document.head.appendChild(t);
  });
</script>
