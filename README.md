# ⏱️ Stopwatch Web Application

A modern and user-friendly **Stopwatch Web Application** built using **HTML, CSS, and JavaScript**. This application allows users to accurately measure time intervals with features like start, pause, reset, and lap time tracking.

---

## 🚀 Features

✅ Start Stopwatch

✅ Pause Stopwatch

✅ Reset Stopwatch

✅ Record Unlimited Lap Times

✅ Real-Time Time Tracking

✅ Responsive Design

✅ Clean and Modern User Interface

✅ Single-Page Application

---

## 🛠️ Technologies Used

* HTML5
* CSS3
* JavaScript (Vanilla JS)

---

## 📂 Project Structure

```text
Stopwatch-Web-App/
│
├── index.html
└── README.md
```

---

## 🎯 Functionality

### ▶️ Start Timer

* Starts the stopwatch.
* Prevents multiple timers from running simultaneously.

### ⏸️ Pause Timer

* Stops the timer without resetting the current time.
* Allows users to resume from where they left off.

### 🔄 Reset Timer

* Resets the stopwatch to `00:00:00`.
* Clears all recorded lap times.

### 🏁 Lap Time Tracking

* Records the current stopwatch time.
* Displays lap times in a scrollable list.
* Supports unlimited lap recordings.

---

## 📸 Preview

Add your project screenshot here:

```text
images/stopwatch-preview.png
```

---

## 💻 How It Works

### Time Calculation

The application tracks:

* Hours
* Minutes
* Seconds

The timer updates every second using:

```javascript
setInterval(() => {
    seconds++;

    if(seconds === 60){
        seconds = 0;
        minutes++;
    }

    if(minutes === 60){
        minutes = 0;
        hours++;
    }

    updateDisplay();

}, 1000);
```

### Lap Recording

Each lap stores the current displayed time and appends it to the lap list.

```javascript
function recordLap() {
    const li = document.createElement("li");
    li.textContent =
    `Lap ${lapCount}: ${display.innerText}`;
}
```

---

## 🎓 Learning Outcomes

Through this project, I learned:

* DOM Manipulation
* Event Handling
* JavaScript Timing Functions
* Dynamic Content Updates
* Responsive Web Design
* User Interface Design
* State Management

---

## 🔮 Future Enhancements

* Millisecond Support
* Dark/Light Theme Toggle
* Export Lap Times
* Local Storage Support
* Keyboard Shortcuts
* Animated Timer Effects

---

## ⚙️ Installation

### Clone the Repository

```bash
git clone https://github.com/your-username/stopwatch-web-app.git
```

### Open Project

```bash
cd stopwatch-web-app
```

### Run Application

Simply open:

```text
index.html
```

in your web browser.

---

## 🤝 Contributing

Contributions, issues, and feature requests are welcome.

Feel free to fork the project and submit a pull request.

---

## ⭐ Support

If you found this project useful, please give it a ⭐ on GitHub.

---

## 👨‍💻 Author

**Bimlesh Kumar**

Aspiring Full Stack Developer

GitHub: https://github.com/your-github-username

LinkedIn: https://linkedin.com/in/your-linkedin-profile
