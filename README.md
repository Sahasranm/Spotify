# 🎶 Spotify Clone

This is a simple Spotify-inspired web app built with **React** and **Context API**. It lets users browse songs, view track details, and control music playback with a sleek, Spotify-like interface.  

---

## 🛠️ Tech Stack

- **Frontend:** React, Tailwind CSS  
- **State Management:** Context API  
- **Icons & Assets:** Local assets folder (`src/assets`)  

---

## 📂 Project Structure


---

## 🧩 Components

### `SongItem.js`

This component displays an individual song and lets users play it by clicking on it.

**Props:**
- `name` (`string`): Song title  
- `image` (`string`): Song cover image URL  
- `desc` (`string`): Short description of the song  
- `id` (`string`): Unique song identifier  

**How it works:**
- Uses `PlayerContext` to access the `playWithId` function  
- Calls `playWithId(id)` when the song is clicked  

---

### `Player.js`

The main music player component. Displays track details and controls for playback.

**Features:**
- Shows current track info: image, name, and description  
- Play/pause button and next/previous track navigation  
- Shuffle, loop, and volume controls  
- Seek bar to track song progress  
- Displays current and total track time  

**Context API:**
- `track`: Current track info (image, name, description)  
- `playStatus`: Whether the song is playing or paused  
- `play()`, `pause()`, `next()`, `previous()`: Playback control functions  
- `time`: Current and total track time  
- `seekBar`, `seekBg`: Refs for the seek bar  

---

## 🚀 How to Run the App

1. **Clone the repository:**

```bash
git clone https://github.com/your-repo/spotify-clone.git
cd spotify-clone
npm install
npm run dev
