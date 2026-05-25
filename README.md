# Smart Grocery Expiry Tracker

A full-stack web application to track grocery expiry dates, reduce food wastage, and make smarter consumption decisions using AI-powered assistance.

---

## 🚀 Features

### Dashboard
- Real-time statistics showing total items, safe items, near-expiry, and expired items
- At-a-glance inventory overview on every visit

### Item Management (CRUD)
- Add, view, update, and delete grocery items
- Each item stores name, quantity, and expiry date

### Expiry Tracking
- Automatically calculates item status on load:
  - ✅ **Safe** — well within expiry
  - ⚠️ **Warning** — nearing expiry
  - ❌ **Expired** — past expiry date

### Smart Planner
- Organizes items based on expiry dates
- Suggests optimal consumption order to minimize waste

### Risk Analysis
- Evaluates overall inventory health
- Classifies risk level as **Low**, **Medium**, or **High** based on expiry distribution

### AI Chat Assistant
- Powered by **OpenAI API**
- Allows users to ask natural language questions about their inventory
- Provides smart consumption suggestions and expiry-based advice in real time

### Voice Input
- Integrated **Web Speech API** for hands-free item addition
- Improves usability for quick grocery entries

---

## 🛠️ Tech Stack

| Layer | Technology |
|-------|-----------|
| Frontend | HTML, CSS, JavaScript |
| Backend | Node.js, Express.js |
| Database | MongoDB |
| AI | OpenAI API |
| Voice | Web Speech API |

---

## 📁 Project Structure

```
expiry-tracker/
├── server.js              # Main Express server
├── package.json
├── .env                   # OpenAI API key and DB config
├── public/
│   ├── index.html         # Main app page
│   ├── style.css
│   └── script.js          # Frontend logic
```

---

## ⚙️ Getting Started

### Prerequisites
- Node.js (v14+)
- MongoDB
- OpenAI API Key

### Installation

1. **Clone the repository**
```bash
git clone https://github.com/23WH1A0507/expiry-tracker.git
cd expiry-tracker
```

2. **Install dependencies**
```bash
npm install
```

3. **Set up environment variables**

Create a `.env` file in the root directory:
```env
OPENAI_API_KEY=your_openai_api_key
MONGODB_URI=your_mongodb_connection_string
PORT=3000
```

4. **Run the server**
```bash
node server.js
```

5. **Open in browser**
```
http://localhost:3000
```

---

## 🤖 AI Chat Assistant

The AI assistant is powered by the OpenAI API. Users can ask questions like:
- *"What items are expiring soon?"*
- *"What should I consume today?"*
- *"How many expired items do I have?"*

The assistant reads the current inventory context and responds with personalized suggestions.

---

## 🎙️ Voice Input

The app uses the browser's built-in **Web Speech API** to capture voice input. Users can speak the item name and details instead of typing, making it faster and more convenient.

---

## 📊 Risk Analysis Logic

| Risk Level | Condition |
|------------|-----------|
| 🟢 Low | Most items are Safe |
| 🟡 Medium | Several items are near expiry |
| 🔴 High | Multiple items are expired or critical |

---

## 🙋‍♀️ Author

**Pravallika Karanam**  
[![GitHub](https://img.shields.io/badge/GitHub-23wh1a0507-black?logo=github)](https://github.com/23wh1a0507)  
[![LinkedIn](https://img.shields.io/badge/LinkedIn-pravallika--karanam-blue?logo=linkedin)](https://linkedin.com/in/pravallika-karanam)

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).
