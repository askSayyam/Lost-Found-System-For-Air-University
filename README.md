# 🏛️ Air University Lost & Found Intelligence System

[![Project Demo](https://github.com/askSayyam/Lost-Found-System-For-Air-University/blob/master/Lost%20%26%20Found.mp4)
*(Click the image above to watch the full system demo)*

Losing an item on a busy campus shouldn't mean it's gone forever. This project is a fully automated, AI-enhanced dashboard designed specifically for the Air University community to intelligently connect lost items with found reports. 

## 🧠 The "Graded Match" Engine
Instead of relying on basic keyword searches, the backend utilizes custom data structures and AI to evaluate matches across four core pillars:

1. **Distance Proximity (Graphs):** Uses **Dijkstra's Algorithm** to calculate the physical distance between where an item was lost and found on the campus map.
2. **Attribute Alignment (Tries):** Instant, optimized matching for exact primary characteristics like Name and Color.
3. **Semantic AI Analysis:** Integrates the **Gemini API** to process human-written descriptions, catching nuanced similarities that traditional searches miss.
4. **Intelligent Automation (Max-Heaps):** All potential matches are scored and ranked using a Max-Heap. The highest-probability match automatically triggers an **n8n webhook**, instantly emailing the original owner.

## 🛠️ Tech Stack
* **Frontend:** TypeScript, React.js (Interactive Campus Map UI)
* **Backend Logic:** C++ 
* **Core Data Structures:** Graphs, Tries, Max-Heaps
* **AI & Automation:** Gemini API, n8n

## 🚀 Quick Start
To run this project locally:
1. Clone the repository: `git clone https://github.com/your-username/air-university-lost-and-found.git`
2. Add your Gemini API key to the `.env` file.
3. Import the `n8n-workflow.json` file into your local n8n instance.
4. Run the frontend: `npm install` followed by `npm start`.
5. Compile and run the C++ backend server.

---
*Built by Sayyam — Bridging algorithmic logic with real-world AI implementation.*
