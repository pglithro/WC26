# 🏆 World Cup Sweepstake Hub

An automated, client-side live dashboard designed to track tournament standings, daily matches, and a dynamic tournament tree mapped against an internal sweepstake player matrix.

---

## ✨ New Features in this Release

### 📅 Live Fixtures & Results Tab
*   **Dynamic Matching:** Automatically extracts and segments matches played yesterday and scheduled for today based on the system anchor timeline.
*   **London Local Time (BST):** Built-in timezone wrapper parsing UTC source datetimes automatically into Europe/London localized presentation formats.
*   **Winner Highlights:** Completed matches dynamically check scorelines, instantly applying a green highlight theme (`.winner-highlight`) and a checkmark (`✓`) next to the winning side.

### ⚡ Knockout Stage
*   **Rebranded Engine:** Replaced the previous "Knockout Bracket" tracking modules with a structurally optimized **"Knockout Stage"** grid layout.
*   **Adaptive Flow:** Columns scale fluidly from the Round of 32 down to the Final match, inheriting sweepstake data allocations and match winner alerts automatically.

---

## 🛠️ Debugging & Simulation

The dashboard contains fallback testing switches directly accessible through URL query string parameters:

| URL Parameter | Action |
| :--- | :--- |
| `?debug=true` | Injects an administrative log console above the standings table showing exact parsing structures and string match flags. |
| `?testko=true` | Force-injects mock programmatic datasets across all brackets to easily test layout spacing, winner highlight states, and team progression flows. |

*Example layout test link:* `index.html?testko=true&debug=true`

---

## 🚀 Getting Started

1. Save the dashboard code as `index.html`.
2. Open `index.html` directly in any modern web browser. 
3. *Note:* Ensure you have an active internet connection so the script can smoothly download the openfootball match arrays over public API endpoints.
