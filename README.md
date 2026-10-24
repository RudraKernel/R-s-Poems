<div align="center">

# 🌹 Whispers of the Heart

### *A garden where every feeling becomes a poem.*

<p>
  <a href="https://YOUR_USERNAME.github.io/REPO_NAME/"><img src="https://img.shields.io/badge/🌐_Live_Demo-ff6d9d?style=for-the-badge" alt="Live Demo"></a>
  <img src="https://img.shields.io/badge/Poems-180-b4146a?style=for-the-badge" alt="180 poems">
  <img src="https://img.shields.io/badge/Dependencies-0-17000e?style=for-the-badge" alt="Zero dependencies">
  <img src="https://img.shields.io/badge/Mobile-First-ffb3cb?style=for-the-badge&labelColor=17000e" alt="Mobile first">
</p>

<p>
  <img src="https://img.shields.io/github/stars/YOUR_USERNAME/REPO_NAME?style=flat-square&color=ff6d9d" alt="Stars">
  <img src="https://img.shields.io/github/forks/YOUR_USERNAME/REPO_NAME?style=flat-square&color=b4146a" alt="Forks">
  <img src="https://img.shields.io/github/last-commit/YOUR_USERNAME/REPO_NAME?style=flat-square&color=ffb3cb" alt="Last commit">
  <img src="https://img.shields.io/github/license/YOUR_USERNAME/REPO_NAME?style=flat-square&color=ff7baa" alt="License">
</p>

*Little poems for the feelings we cannot always say.*

**✦ Made by Rudra ✦**

[Live Demo](https://YOUR_USERNAME.github.io/REPO_NAME/) · [Report a Bug](https://github.com/YOUR_USERNAME/REPO_NAME/issues) · [Suggest a Poem](https://github.com/YOUR_USERNAME/REPO_NAME/issues)

</div>

---

> **Setup note:** replace `YOUR_USERNAME` and `REPO_NAME` everywhere in this file with your GitHub username and repository name (use Find & Replace). Then delete this note.

---

## 📑 Table of Contents

- [About](#-about)
- [Preview](#-preview)
- [Features](#-features)
- [Getting Started](#-getting-started)
- [Deploy with GitHub Pages](#-deploy-with-github-pages)
- [Controls](#-controls)
- [Add Your Own Poems](#️-add-your-own-poems)
- [Customize](#-customize)
- [Performance Notes](#-performance-notes)
- [Project Structure](#-project-structure)
- [Contributing](#-contributing)
- [License](#-license)

---

## ✨ About

**Whispers of the Heart** is a dreamy, rose-themed poetry website. You step through a glowing intro screen, enter the garden, and find **180 short poems**, each a four-line whisper. Tap a poem and its lines fade in one by one while petals drift across the screen.

It is a **single `index.html` file** with no frameworks, no build step and no libraries. It is built **mobile-first** and runs smoothly on phones.

---

## 📸 Preview

<!--
Add screenshots to an "assets" folder, then remove this comment block and uncomment the table below.

<table>
  <tr>
    <td align="center"><img src="assets/intro.png" width="240" alt="Intro screen"><br><sub>Intro</sub></td>
    <td align="center"><img src="assets/garden.png" width="240" alt="Poem grid"><br><sub>The Garden</sub></td>
    <td align="center"><img src="assets/poem.png" width="240" alt="Poem view"><br><sub>A Poem</sub></td>
  </tr>
</table>
-->

👉 **[Open the live site](https://YOUR_USERNAME.github.io/REPO_NAME/)** (best viewed on a phone).

---

## 🌸 Features

| | Feature | Details |
|---|---|---|
| 🌹 | **Animated intro** | Glowing orbs, floating roses and a soft entrance |
| 📖 | **180 poems** | Feelings, nature, and little everyday objects |
| 🔍 | **Live search** | Search by title, word or any line of a poem |
| 💫 | **Line-by-line reveal** | Each poem fades in one line at a time |
| 👆 | **Swipe navigation** | Swipe left or right in a poem to change poems |
| 🌸 | **Petal effects** | Falling petals plus a petal burst when you tap |
| ✨ | **Custom cursor** | Glowing cursor with a trail (desktop only) |
| 📱 | **Mobile-first** | 2-column grid, big touch targets, notch-safe layout |
| ⚡ | **Performance tuned** | Only GPU-friendly animations, nothing heavy |
| ♿ | **Reduced-motion aware** | Fewer animations for people who prefer less motion |

---

## 🚀 Getting Started

No installation, no `npm install`, no build.

```bash
# 1. Clone the repository
git clone https://github.com/YOUR_USERNAME/REPO_NAME.git

# 2. Go into the folder
cd REPO_NAME

# 3. Open index.html in your browser
#    macOS:   open index.html
#    Windows: start index.html
#    Linux:   xdg-open index.html
```

Or just download `index.html` and double-click it.

---

## 🌍 Deploy with GitHub Pages

Free hosting straight from this repo:

1. Push `index.html` to the `main` branch.
2. Open your repository on GitHub and go to **Settings → Pages**.
3. Under **Build and deployment**, set **Source** to **Deploy from a branch**.
4. Choose the **`main`** branch and the **`/ (root)`** folder, then click **Save**.
5. Wait a minute or two. Your site will be live at:

```
https://YOUR_USERNAME.github.io/REPO_NAME/
```

Every time you push a change to `main`, the site updates automatically.

---

## 🎮 Controls

| Action | Phone 📱 | Desktop 🖥️ |
|---|---|---|
| Open a poem | Tap a card | Click a card |
| Next poem | Swipe left, or tap **Next →** | `→` key or **Next →** |
| Previous poem | Swipe right, or tap **← Prev** | `←` key or **← Prev** |
| Close a poem | Tap **×** or tap outside the box | `Esc`, **×**, or click outside |
| Search | Type in the search bar | Type in the search bar |

---

## ✍️ Add Your Own Poems

All poems live in one array near the top of the `<script>` section in `index.html`:

```js
const poems = [
  { title: "Morning", lines: [
      "The sun slips softly through the trees,",
      "Painting gold across the breeze.",
      "A new day whispers, “Begin,”",
      "And hope awakens from within."
  ]},
  // ...
];
```

To add a poem, put a comma after the last one and add:

```js
{ title: "Your Title", lines: [
    "First line,",
    "Second line,",
    "Third line,",
    "Fourth line."
]}
```

The grid, search, counter and navigation update automatically. The poem counter (`1 / 180`) also adjusts to the new total.

> 💡 If you add many poems, update the **Poems** badge at the top of this README.

---

## 🎨 Customize

| I want to... | Do this |
|---|---|
| Change the name | Search for `Made by Rudra` in `index.html` and replace it |
| Change the colors | Edit the pink `rgba(255, …)` values in the CSS |
| Change the petals | Edit `fallTypes` and `burstTypes` in the script |
| More or fewer falling petals | Edit `MAX_FALLING` and `FALL_INTERVAL` |
| Slow down the poem reveal | In `openPoem`, change `0.2 + i * 0.4` (seconds per line) |

---

## ⚡ Performance Notes

Phones are picky, so the site follows a few rules:

- **Only `transform` and `opacity` are animated.** The GPU handles these without layout work.
- **No blur or heavy filters** on cards or overlays.
- **Off-screen cards are skipped** with `content-visibility: auto`, so 180 cards stay light.
- **Petals are capped and removed** as soon as they finish animating.
- **The intro is deleted** from the page after you enter, freeing all its animations.
- **Search is debounced**, so typing never stutters.
- **The custom cursor and hover effects** only load on devices with a mouse.

---

## 📁 Project Structure

```
📦 REPO_NAME
 ┣ 📂 assets        ← (optional) screenshots for the README
 ┣ 📜 index.html    ← the whole website: HTML + CSS + JS + poems
 ┣ 📜 README.md     ← you are here
 ┗ 📜 LICENSE       ← (optional) see below
```

---

## 🤝 Contributing

Suggestions are welcome.

- **Found a bug?** [Open an issue](https://github.com/YOUR_USERNAME/REPO_NAME/issues).
- **Have a poem to share?** Open an issue, or fork the repo, add it to the `poems` array, and send a pull request.

Please keep poems original and four lines long to match the rest of the garden.

```bash
git checkout -b add-my-poem
git commit -am "Add poem: Your Title"
git push origin add-my-poem
```

Then open a Pull Request on GitHub.

---

## 📄 License

Add a `LICENSE` file to your repo to make the terms clear (on GitHub: **Add file → Create new file → name it `LICENSE`**, and choose a template such as MIT). Until you do, the code is all rights reserved by default.

---

<div align="center">

### 💌 Made with care by Rudra

*Every heart has a story.* 🌹

If you liked the garden, a ⭐ on the repo means a lot.

**✦ Made by Rudra ✦**

</div>
