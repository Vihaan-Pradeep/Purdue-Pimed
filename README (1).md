# PiMed Website

Official website for the **Purdue in Indianapolis Medical Association (PiMed)** — a student organization at Purdue University Indianapolis connecting pre-med and health science students with professionals, opportunities, and community.

🌐 **Live site:** `https://yourusername.github.io/pimed-website`

---

## Pages

| Page | What's on it |
|------|-------------|
| **Home** | Hero, what we do, recent events highlight, join CTA |
| **Mission** | Mission statement, 4 pillars, photo gallery |
| **Team** | Advisor, executive board, on-call officers |
| **Events** | Past events (filterable), upcoming events, MCAT prep banner |
| **Get Involved** | BoilerLink signup, board application, GroupMe, newsletter, socials |
| **Map** | Interactive Indianapolis map — hospitals, med schools, BME, medtech |

---

## How to Edit

Everything is in one file: `index.html`. Open it in any text editor (VS Code recommended) or edit directly on GitHub using the pencil icon.

### Common edits

**Team members** — find `const TEAM_DATA` near the bottom of the file. Each entry looks like:
```js
{ name:"President", role:"President", initials:"PR", bio:"..." }
```
Update `name`, `initials`, and `bio` with real info.

**Events** — find `const EVENTS_DATA`. Each entry looks like:
```js
{ title:"Blood Drive", desc:"...", type:"community", month:"APR", day:"12", year:2025, upcoming:false }
```
Set `upcoming: true` for future events. Types: `community`, `academic`, `clinical`, `social`.

**Map locations** — find `const locations` inside the `initMap()` function. Each entry looks like:
```js
{ lat:39.768, lng:-86.158, name:"Hospital Name", type:"hospital", desc:"..." }
```
Types: `hospital`, `medschool`, `bme`, `medtech`.

**Photos** — search for `photo-placeholder` in the HTML and replace those divs with `<img>` tags pointing to your image files.

**Social media links** — search for `href="https://instagram.com/purdue.pimed"` etc. and update with real URLs.

**GroupMe link** — search for `Join GroupMe` and replace the `href="#"` with the actual GroupMe invite link.

---

## Tech Stack

- Plain HTML, CSS, JavaScript — no frameworks, no build step
- [Leaflet.js](https://leafletjs.com/) for the interactive map
- [Google Fonts](https://fonts.google.com/) — DM Serif Display + DM Sans
- Hosted on GitHub Pages (free)

---

## Updating the Site

1. Edit `index.html` (locally or on GitHub)
2. If editing locally, upload the new file to GitHub
3. Changes go live automatically within ~30 seconds

For bigger changes, paste the file into a Claude chat and describe what you want — Claude can make targeted edits without rewriting the whole file.

---

## Contact

📧 pimed@purdue.edu  
📸 [@purdue.pimed](https://instagram.com/purdue.pimed)  
📍 Science, Engineering and Technology Building, Indianapolis, IN 46202
