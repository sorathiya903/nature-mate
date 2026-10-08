# 🌿 NatureMate — Touch Grass Edition

A game that uses your screen to make you leave the screen.

NatureMate is a mobile-first outdoor game that turns the real world into your game board.

You get an outdoor quest, step outside, point your camera at something, and let browser-based AI check whether you found it.

The goal isn’t to spend more time on the screen. It’s to give you a reason to look away from it.

## 🎮 Play

[🌿 Play NatureMate](https://naturemate.netlify.app/game)

⸻

✨ How It Works

1. Get a quest
    NatureMate gives you something to find outside.
2. Go outside
    Take your phone with you and look around.
3. Point & capture
    Use the camera to capture what you found.
4. AI checks it
    Browser-based object detection analyzes the image.
5. Earn rewards
    Complete the quest to earn XP, coins, and streak progress.
6. Keep exploring
    Found or skipped objects don’t return to your quest pool.

⸻

🌱 What’s Inside

🔎 Outdoor Quests

Find real-world objects using your camera.

🤖 Browser AI

NatureMate uses object detection directly in the browser to recognize supported objects.

The AI runs client-side, so the core game doesn’t require a custom backend for camera detection.

❤️ 3 Lives

You have three lives.

Skipping a quest costs one life, while simply failing to detect the requested object does not.

🔥 Streaks

Keep completing quests to maintain your streak.

⭐ XP & Coins

Successful discoveries reward XP and coins as you progress.

🚫 No Repeated Quests

Once an object is successfully found or skipped, it won’t be selected again during that game.

🏃 Touch Grass Run

A separate 10-minute challenge mode where you try to complete a set of outdoor targets before time runs out.

⸻

🧠 AI in the Browser

NatureMate uses Transformers.js with a browser-compatible YOLOS object-detection model.

The basic flow is:

📷 Camera
    ↓
🖼️ Image
    ↓
🧠 YOLOS
    ↓
🔍 Object Detection
    ↓
🎯 Quest Verification
    ↓
⭐ XP + 🪙 Coins

No custom AI backend is required for the game’s object-detection workflow.

⸻

📱 Built for Mobile

NatureMate is designed primarily for phones because the camera is part of the gameplay.

It is designed to work across modern:

* Android browsers
* iOS browsers
* Desktop browsers

Camera permissions are required for gameplay.

⸻

🛠️ Tech Stack

* HTML
* CSS
* JavaScript
* Transformers.js
* YOLOS object detection
* ONNX Runtime Web / WASM
* Browser Camera API
* Netlify

The project intentionally keeps the architecture lightweight and client-side.

⸻

🚀 Run Locally

Clone the repository:
```
git clone https://github.com/sorathiya903/nature-mate.git
```
```
cd nature-mate
```
Then serve the frontend using any local HTTP server.

For example:
```
python -m http.server 8000
```
Open:
```
http://localhost:8000
```
Camera access may require a secure context such as HTTPS or a local development environment supported by the browser.

⸻

📂 Project

The main game is currently located in:

frontend/
└── game.html


⸻

🎯 Why I Built It

Most games are designed to keep you looking at the screen.

NatureMate is built around the opposite idea:

The screen gives you the mission.
The real world completes it.

Ideally, you shouldn’t spend hours playing NatureMate.

You should open it, get a quest, go outside, find something, complete it, and keep exploring.

⸻

🔮 What’s Next

NatureMate is still evolving.

Possible future improvements include:

* More outdoor targets
* More game modes
* Better object relationships
* More challenges
* Improved mobile performance
* More ways to explore the real world through the game

⸻

🤝 Contributing

Found a bug or have an interesting idea?

Feel free to open an issue or submit a pull request.

Suggestions for new game mechanics are especially welcome.

⸻

📜 License

See the repository’s license file for the current licensing terms.

⸻

👨‍💻 Author

Aditya Sorathiya

Student developer building projects around web development, Python, AI, and the web.

Live: https://naturemate.netlify.app
