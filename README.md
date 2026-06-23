# 🏆 World Cup Sweepstake Standings Tracker

A lightweight, zero-dependency web application that displays live World Cup group standings and automatically tags each country with its assigned sweepstake player. 

The site is built to run entirely in the browser and is optimized for hosting via GitHub Pages without encountering CORS (Cross-Origin Resource Sharing) restrictions.

## 🚀 Live Demo
View your tournament dashboard here: [https://pglithro.github.io/WC26/](https://pglithro.github.io/WC26/)

---

## 🛠️ How It Works

1. **Live Data Fetching:** The app queries an open-source, CORS-friendly tournament data stream updated live on GitHub.
2. **Dynamic Mapping:** A JavaScript configuration block maps every competing nation to a player based on your custom draft slips.
3. **Automated Sorting:** The dashboard renders organized group cards, auto-calculating rankings dynamically by Points (Pts) and Goal Difference (GD).

---

## 🎲 Customizing for Future Sweepstakes

You can easily repurpose this codebase for future tournaments, different sports, or completely different player rosters. All modifications take place in a single dictionary block inside the `index.html` file.

### Step-by-Step Roster Updates:

1. Open your `index.html` file in a text editor.
2. Scroll down to the `<script>` tag near the bottom and locate the `sweepstakeData` object:

```javascript
// Sweepstake configuration matching image_25d644.png
const sweepstakeData = {
    "France": "Alexis", 
    "Curaçao": "Alexis",
    "Spain": "Savir", 
    "Haiti": "Savir",
    // Add or modify your pairs here...
};
