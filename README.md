📧 Email Writer Assistant
AI-powered email reply generator built with Spring Boot, React.js, Vite, Spring AI, and Gemini API. It intelligently crafts email replies based on the original email and the selected tone.

🚀 Features
🔥 Real-time AI email reply generation using Google Gemini API 2.0

🧠 Choose your tone (Casual, Formal, Friendly, etc.)

📩 Paste an original email and instantly get a relevant reply

💡 Built with Spring AI & React (Vite-based frontend)

🌐 Chrome extension integration for Gmail

🧪 Backend tested with Postman

⚙️ Customizable with .env or environment variables

🖼️ Screenshots
🎯 Chrome Extension Enabled

🧠 Web App Interface

📥 Gmail Integration (Draft)

⚙️ IntelliJ Run Configuration

🛠️ Tech Stack
Layer	Tech Used
Frontend	React.js, Vite, JavaScript
Backend	Spring Boot, Spring AI
AI API	Gemini API (v2.0 - generative)
Testing	Postman
Extension	Chrome Extension (Manifest V3)
IDE	IntelliJ IDEA

⚙️ Environment Variables
Set the following variables in your run configuration or .env:

ini
Copy
Edit
GEMINI_URL=https://generativelanguage.googleapis.com/v1beta/models/gemini-pro:generateContent
GEMINI_API_KEY=your_gemini_api_key_here
🔧 How to Run Locally
Clone the repository

bash
Copy
Edit
git clone https://github.com/your-username/email-writer-assistant.git
cd email-writer-assistant
Start Backend
Make sure Java 17+ is installed.
Run with IntelliJ or:

bash
Copy
Edit
./mvnw spring-boot:run
Start Frontend

bash
Copy
Edit
cd email-writer-react
npm install
npm run dev
Use Postman (Optional)

Import the API collection

Test endpoint: POST /api/generate-reply

Load Chrome Extension

Go to chrome://extensions/

Enable Developer Mode

Click Load unpacked and select the extension folder

🧠 How It Works
User inputs an original email and selects the tone.

Frontend sends data to Spring Boot backend.

Spring AI sends a request to Gemini API with prompt tuning.

Generated reply is returned to the frontend and shown in the UI.

User can copy the response or auto-fill Gmail draft via Chrome Extension.

✨ Example Output
Input:

Hey there - this is John here. We connected at the AWS summit last week. How is it going with your startup?

Tone: Casual
Output:

Hi John,
Great to hear from you! It was good meeting you at the AWS Summit last week.
Things are moving along with the startup. Definitely keeping busy! How was the summit for you overall?

📝 Future Enhancements
✉️ Direct Gmail API integration

🗣️ Voice-to-email prompt

🌍 Multilingual support

📊 Dashboard for email history

👤 Author
Ashwin Maheshkumar

LinkedIn • GitHub

📄 License
MIT License
