# 🎵 Melodies — Personal Music Player

> *All the Best Songs in One Place*

A fully responsive, feature-rich personal music player built with pure **HTML, CSS, and JavaScript** — zero frameworks, zero dependencies except Font Awesome icons. Designed with a dark pink/purple aesthetic inspired by modern streaming platforms.

---

## ✨ Features

### 🎧 Music Player
- Real audio playback using the native Web Audio API (`new Audio()`)
- **Play / Pause** toggle with live icon swap
- **Next & Previous** track navigation
- **Seek** — click anywhere on the progress bar to jump
- **Live timestamps** — current time and total duration update in real time
- **Shuffle** mode — randomises the play queue
- **Loop** mode — repeats the current song on end
- **Volume control** slider with dynamic icon (mute / low / high)
- **Auto-advance** — automatically plays next song when current ends
- **Like / Heart** button — synced between player bar and trending table

### 🗂️ Song Library
- 37 curated personal songs across genres — Bollywood, Hindi Indie, Devotional, International
- **Weekly Top Songs** horizontal scroll section
- **New Releases** horizontal scroll section
- **Trending Songs** table with rank, release date, album, duration, and like button
- Trending row highlights pink when that song is currently playing

### 📱 Fully Responsive Design
| Breakpoint | Layout |
|---|---|
| Desktop (> 900px) | Sidebar + main content side by side, full player bar |
| Tablet (≤ 900px) | Sidebar becomes slide-in drawer overlay, condensed topbar |
| Mobile (≤ 600px) | Single column, stacked 2-row player (track info + controls) |
| Small phones (≤ 380px) | Compact single-row mini player (thumbnail + prev/play/next only) |

### 🎨 Design
- Dark theme — `#0a0a0a` background with `#ff00cc` pink and `#9900ff` purple accents
- Smooth hover effects on all song cards (lift + pink glow)
- Play overlay appears on card hover
- Gradient progress bar (pink → purple)
- Sidebar drawer with backdrop blur overlay on mobile
- Sticky topbar with glassmorphism blur effect
- Custom scrollbar styling

---

## 📁 Project Structure

```
melodies/
│
├── melodies_fixed.html        # Main application (single file)
│
└── My_Favorite_Songs/         # Your MP3 files go here
    ├── Aari Aari (...).mp3
    ├── Aditya Rikhari - FAASLE.mp3
    ├── Gehra Hua.mp3
    └── ... (37 songs total)
```

> ⚠️ The `My_Favorite_Songs/` folder **must be in the same directory** as `melodies_fixed.html` for audio to work.

---

## 🚀 How to Run

No build step, no server required for most browsers.

**Option 1 — Direct open (simplest)**
```
Double-click melodies_fixed.html
```
> Note: Some browsers block local audio loading via `file://`. If songs don't play, use Option 2.

**Option 2 — Local server (recommended)**

Using Python:
```bash
# Python 3
python -m http.server 8080

# Then open:
http://localhost:8080/melodies_fixed.html
```

Using Node.js:
```bash
npx serve .
```

Using VS Code — install the **Live Server** extension, right-click `melodies_fixed.html` → *Open with Live Server*.

---

## 🎵 Song List

| # | Title | Artist | Duration |
|---|---|---|---|
| 1 | Aari Aari | Dhurandhar The Revenge | 3:30 |
| 2 | FAASLE | Aditya Rikhari | 3:36 |
| 3 | Akeli Laila | Baaghi 4 | 2:40 |
| 4 | Bairan | Banjaare | 2:30 |
| 5 | Bairi | Virat, Miss Parul | 3:14 |
| 6 | Darkside x Aaja Sanam | Lata Mangeshkar & Neoni | 3:05 |
| 7 | Dhaaga | Nilotpal Bora | 3:46 |
| 8 | Dhurandhar - Title Track | Shashwat Sachdev, Hanumankind | 2:58 |
| 9 | Finding Her | Bharath, Kushagra & Saaheal | 3:27 |
| 10 | Raanjhan | Parampara Tandon | 3:27 |
| 11 | Ganga Ke Kinare | Bunny Sagar | 3:27 |
| 12 | Gehra Hua | Arijit Singh | 3:51 |
| 13 | Haan Ke Haan | Zendria | 2:21 |
| 14 | Jalwa | Carryminati | 3:29 |
| 15 | Unse Jaake Kehdo | Justh | 3:02 |
| 16 | Laal Pari | Yo Yo Honey Singh | 3:04 |
| 17 | Madhurashtakam | Zendria | 5:01 |
| 18 | Main Bola Hey | Karthik Rao | 2:50 |
| 19 | Main Tumhara | A.R. Rahman, Jonita Gandhi | 2:46 |
| 20 | Naam Chale | Vikram Sarkar | 2:29 |
| 21 | O Re Manwa | Meghna Mishra | 3:40 |
| 22 | Om Namo Bhagavate Vasudevaya | Vijay Prakash, Sanjith Hegde | 2:46 |
| 23 | Paisa | Mellow-D, Sachin-Jigar, Vishal Dadlani | 3:06 |
| 24 | Radha Rani Lage | Zendria | 3:22 |
| 25 | Shararat | Jasmine Sandlas, Shashwat Sachdev | 3:49 |
| 26 | Sunehra | Jai Dhir | 3:27 |
| 27 | Badli Si Hawa Hai | Arijit Singh | 2:47 |
| 28 | Theme Song – Scam 1992 | Achint | 2:58 |
| 29 | Shree Raghuvar Komal Nayan | Zendria | 3:33 |
| 30 | Shree Ram Stuti | Kids Performance | 3:08 |
| 31 | Dooron Dooron | Meghdeep Bose, Paresh Pahuja | 4:05 |
| 32 | Matkar Maya Ko Ahankar | Kabir Café | 6:05 |
| 33 | Tenu Sang Rakhna | Achint, Arijit Singh, Anumita Nadesan | 3:02 |
| 34 | Sahiba | Stebin Ben, Jasleen Royal | 3:37 |
| 35 | Rasputin | Boney M | 3:40 |
| 36 | Shape of You | Ed Sheeran | 4:23 |
| 37 | O Ri Chiraiya | Swanand Kirkire | 4:33 |



---

## 🛠️ Tech Stack

| Technology | Usage |
|---|---|
| HTML5 | Structure and semantic markup |
| CSS3 | Styling, CSS Grid layout, Flexbox, CSS Variables, Media Queries |
| Vanilla JavaScript (ES6+) | All interactivity, audio engine, DOM manipulation |
| Web Audio API | Native `Audio` object for real MP3 playback |
| Font Awesome 6.5 | Icons (via CDN) |

**No frameworks. No build tools. No npm. Just open and play.**

---

## 📐 CSS Architecture

All styles live in a single `<style>` block using **CSS custom properties (variables)** defined in `:root`:

```css
:root {
  --bg:           #0a0a0a;   /* page background */
  --sidebar:      #111111;   /* sidebar surface */
  --accent-pink:  #ff00cc;   /* primary accent */
  --accent-purple:#9900ff;   /* secondary accent */
  --surface:      #181818;   /* card background */
  --border:       #2a2a2a;   /* divider colour */
}
```

To change the colour theme, edit only these variables.

---

## 🐛 Known Limitations

- **No backend** — likes, play counts, and queue state reset on page refresh
- **Local files only** — audio paths are relative; hosting requires uploading MP3s too
- **No playlist creation UI** — library sections are static (can be extended in JS)
- Songs with special characters (｜, ：) in filenames work locally but may need URL encoding on some web servers

---

## 🔮 Possible Future Improvements

- [ ] `localStorage` persistence for liked songs and volume preference
- [ ] Search bar that filters songs live across all sections
- [ ] Create / delete custom playlists
- [ ] Keyboard shortcuts (Space = play/pause, ← → = seek, N = next)
- [ ] Waveform visualiser using Web Audio API `AnalyserNode`
- [ ] PWA support — install as an app on mobile

---

## 👤 Author

**Rajat**
Personal music player project — built iteratively with progressive design and mobile-first responsive fixes.

---

## 📄 License

This project is for **personal use only.**
All songs belong to their respective artists and labels.
No copyright infringement intended.
