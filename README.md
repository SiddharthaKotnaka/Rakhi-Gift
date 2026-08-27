# 🎀 Raksha Bandhan Memory Website

A cinematic, personal, interactive surprise website from a brother to his sister.

## 🚀 Quick Start

1. Open `index.html` in your browser — that's it!
2. No build tools, no frameworks, no installation needed.

## 📸 Adding Your Photos

1. Put your 15 photos in the `images/` folder
2. Name them: `photo01.jpeg`, `photo02.jpeg`, ... `photo15.jpeg`
3. Open `script.js` and find the **PERSONALIZATION** section at the top
4. Update the captions in the `memories` array

### Photo Tips
- **Recommended size**: 800×600px or similar (4:3 ratio works best)
- **Format**: JPG, PNG, or WebP all work
- **File size**: Keep each photo under 500KB for fast loading
- If your photos are different dimensions, they'll be cropped to fit (using `object-fit: cover`)

## ✏️ Personalization

Everything you need to customize is in **one place** — the `CONFIG` object at the top of `script.js`:

### Names
```js
sisterName: 'Didi',        // Your sister's name or nickname
brotherName: 'Your Brother', // Your name
year: '2026',               // Year
```

### Photo Captions
Each memory in the `memories` array has:
```js
{
  image: 'images/photo01.jpeg',  // Photo file path
  title: 'The Beginning',       // Short title
  caption: 'Where it all started.', // Description
  year: '200X'                  // Optional year
}
```

### Personal Letter
Edit the `letter` field with your own words:
```js
letter: `Dear Didi,

Your personal letter goes here...

Write from the heart.`,
```

### Final Photo
The "best" photo shown at the dramatic end:
```js
finalPhoto: { image: 'images/photo15.jpeg', alt: 'Our favorite memory' },
```

### Sibling Fight Messages
Customize the funny fight dialog:
```js
fightMessages: [
  'Give me the remote.',
  'No.',
  // Add your own!
],
```

## 🎵 Adding Music

1. Put your music file in the `music/` folder as `music.mp3`
2. The music button will appear automatically
3. If no music file exists, the button hides itself — no errors

## 📁 File Structure

```
rakhi/
├── index.html      ← The website (open this!)
├── style.css       ← All styles
├── script.js       ← All interactions + CONFIG
├── README.md       ← You're reading this
├── images/
│   ├── photo01.jpeg
│   ├── photo02.jpeg
│   ├── ...
│   └── photo15.jpeg
└── music/
    └── music.mp3   ← Optional
```

## 🌐 Deploying Online

### Free Options
- **GitHub Pages**: Push to a GitHub repo, enable Pages in Settings
- **Netlify**: Drag & drop the folder at netlify.com/drop
- **Vercel**: Import the folder at vercel.com

### Sharing
After deploying, you'll get a URL like `https://yourname.github.io/rakhi/`  
Send it to your sister! 🎉

## 🔧 Troubleshooting

| Issue | Fix |
|-------|-----|
| Photos not showing | Check file names match exactly (case-sensitive) |
| Music not playing | Browsers require a user click before playing audio |
| Animations laggy | Reduce photo file sizes to under 300KB each |
| Text looks weird | Make sure you have internet (fonts load from Google) |

## 🎨 Design Features

- **6 Chapters**: Opening → Childhood → Memories → Chaos → Letter → Rakhi → Finale
- **15-Photo Gallery**: Dynamic scrapbook with lightbox viewer
- **Interactive Elements**: Photo reveal, sibling fight simulator, rakhi interaction
- **Easter Eggs**: Tap the heart 5 times, tap the rakhi icon 3 times 🤫
- **Responsive**: Works on phones, tablets, laptops, and desktops
- **Accessible**: Keyboard navigation, screen reader support, reduced motion
- **No Dependencies**: Pure HTML + CSS + JavaScript

## ❤️ Made with love, memories & a little bit of sibling chaos.
