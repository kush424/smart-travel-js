
# 🌍 Smart Travel Planner

A prompt-driven JavaScript travel planner that demonstrates beginner-friendly concepts like arrays, loops, functions, conditionals, and DOM manipulation — all wrapped in a clean, modern UI with icons and a scenic background.

📋 Table of Contents
- Overview
- Features
- Installation
- Usage
- Planner Flow (Logic Included)
- Technologies Used
- Project Structure
- Contributing
- License
- Author
- Screenshots
- Why This Project?

🎯 Overview
The Smart Travel Planner is an interactive, browser-based project that helps users plan a trip by collecting destinations, total budget, and number of days using prompt dialogs. It then computes the trip type and hotel recommendation, and displays a styled summary on the webpage while logging details to the console.

✨ Features
- ✅ Prompt-Driven Interface
  - Simple prompts guide the user step-by-step (destinations, budget, days).
- ✅ Clean Summary UI
  - Modern card design with icons, background image, and Poppins font.
- ✅ Core Travel Logic
  - Budget advice, trip type by days, and hotel suggestion based on budget/day.
- ✅ Multiple Output Methods
  - Summary displayed via innerHTML.
  - All details logged to the browser console.
  - alert() for completion notification.
- ✅ Modern JavaScript (ES6+)
  - let, const, and template literals used for clarity and readability.
- ✅ No Build Tools
  - Pure HTML, CSS, and JavaScript (Font Awesome & Google Fonts via CDN).

💻 Installation
Clone the repository:
```bash
git clone https://github.com/YOUR_USERNAME/smart-travel-planner.git
```
Navigate to the project directory:
```bash
cd smart-travel-planner
```
Open the HTML file:
- Double-click index.html to open it in your default browser.

📖 Usage
- Open index.html in your browser.
- Enter 3 destinations when prompted.
- Enter your total budget (₹).
- Enter number of travel days.
- See the styled “Travel Summary” on the page.
- Open Developer Tools → Console to view logs.
- You’ll see an alert: “Smart Travel Plan Ready!” at the end.

🧩 Planner Flow (Logic Included)
1) Destination Collector (Array + Loop)
- A for loop runs 3 times and pushes entered destinations into the places array.

2) Budget Advisor (Conditionals)
- Budget ranges determine travel advice:
  - < ₹10,000 → “Plan a short domestic trip.”
  - ₹10,000–₹50,000 → “You can plan a long domestic trip.”
  - > ₹50,000 → “International trip possible!”

3) Trip Type by Days (Conditionals)
- < 3 days → “Weekend Getaway.”
- 3–7 days → “Perfect Holiday Trip.”
- > 7 days → “Extended Vacation.”

4) Hotel Suggestion (Function)
Uses per-day budget to recommend a hotel category.
```js
function hotelSuggestion(budget, days) {
  if (days === 0) return "Not applicable.";
  let perDay = budget / days;
  if (perDay < 2000) return "Budget Hotels.";
  else if (perDay <= 5000) return "Mid-range Hotels.";
  else return "Luxury Hotels.";
}
// Example:
// Input: budget = 35000, days = 5 → perDay = 7000 → "Luxury Hotels."
```

5) Output Rendering
- Summary is injected into the #summary-output div using innerHTML with template literals.
- Results also logged via console.log for learning and debugging.
- Final alert confirms completion.

🛠️ Technologies Used
| Technology         | Purpose                                                     |
|--------------------|-------------------------------------------------------------|
| HTML5              | Structure and content                                       |
| CSS3               | Clean, modern UI (card, background, fonts)                  |
| JavaScript (ES6+)  | Core logic, functions, loops, conditionals, template literals |
| Browser APIs       | prompt, alert, console.log, innerHTML for I/O               |
| Google Fonts       | Poppins (via CDN)                                           |
| Font Awesome       | Icons in the summary (via CDN)                              |

📁 Project Structure
```
smart-travel-planner/
│
├── index.html   # Contains HTML, CSS (in <style>), and JS (in <script>)
└── README.md    # Project documentation
```

🤝 Contributing
Contributions, issues, and suggestions are welcome!

1) Fork the repository  
2) Create a feature branch: git checkout -b feature/YourFeature  
3) Commit your changes: git commit -m "Add YourFeature"  
4) Push to the branch: git push origin feature/YourFeature  
5) Open a Pull Request

📄 License
This project is open source and available under the MIT License. See the LICENSE file for details.

👨‍💻 Author
Created by [patel kush] — passionate about building simple and effective learning projects.  
GitHub: https://github.com/YOUR_USERNAME  
Email: kushpatel8543@gmail.com

📎 Screenshots
<img width="439" height="155" alt="image" src="https://github.com/user-attachments/assets/7799a389-e3ed-4148-9e4a-ba0dda939964" />
<img width="1899" height="925" alt="image" src="https://github.com/user-attachments/assets/d2ee5232-3a9c-4b59-a3cd-800e979cb49a" />
<img width="354" height="130" alt="image" src="https://github.com/user-attachments/assets/6eb20dbc-9d67-463b-9f3b-095fb84dadfb" />

- UI Summary (screenshots/ui-summary.png)
- Console Logs (screenshots/console-logs.png)



🌟 Why This Project?
- Perfect for beginners practicing arrays, loops, functions, and conditionals.
- Hands-on experience with prompt-based user input and DOM updates.
- Clean UI helps present your logic professionally for assignments or demos.

✅ Built with ❤️ to make learning JavaScript fun and practical!
