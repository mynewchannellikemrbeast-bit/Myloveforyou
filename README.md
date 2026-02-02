# Will You Be My Valentine? 💖

An interactive mobile-first Valentine's Day website with playful animations, sound effects, and romantic surprises!

## ✨ Features

- **7 Interactive Pages**: From introduction to the big question and celebration
- **Special NO Button Mechanic**: The NO button runs away and triggers a fun screen break effect
- **Romantic Sound Effects**: Perfectly timed audio for each interaction
- **Animated Gradient Background**: Smooth flowing pink and red gradients
- **Couple GIFs**: Transparent animated decorations on each page
- **Fully Responsive**: Mobile-first design works on all screen sizes (320px - 1440px+)
- **Easy Customization**: All assets are editable from the GitHub repo

## 🎯 Page Flow

1. **Introduction** - Welcome message with your custom text
2. **Heart Reveal** - Click the heart to reveal your first message
3. **Letter Reveal** - Open the envelope for your second message
4. **Stars Reveal** - Touch the stars for your third message
5. **Flowers Reveal** - Pick the flowers for your fourth message
6. **The Big Question** - "Will you be my valentine?" with YES/NO buttons
7. **Success!** - Celebration page with confetti

## 📝 How to Customize

### 1. Add Your Handwritten Messages

Open `index.html` and search for `(add text)` - there are 5 placeholders:

- **Page 2** (Heart Reveal): Replace line with `id="reveal-1-message"`
- **Page 3** (Letter Reveal): Replace line with `id="reveal-2-message"`
- **Page 4** (Stars Reveal): Replace line with `id="reveal-3-message"`
- **Page 5** (Flowers Reveal): Replace line with `id="reveal-4-message"`
- **Page 7** (Success): Replace the success message placeholder

**Example:**
```html
<!-- Before -->
<div class="revealed-message message-placeholder" id="reveal-1-message">
    (add text)
</div>

<!-- After -->
<div class="revealed-message message-placeholder" id="reveal-1-message">
    You make my heart skip a beat every single day! 💕
</div>
```

### 2. Replace GIFs

Navigate to `assets/gifs/` and add your own animated couple GIFs:

- `couple-1.gif` - Page 2 (Heart Reveal)
- `couple-2.gif` - Page 3 (Letter Reveal)
- `couple-3.gif` - Page 4 (Stars Reveal)
- `couple-4.gif` - Page 5 (Flowers Reveal)
- `couple-5.gif` - Page 6 (The Question)
- `couple-success.gif` - Page 7 (Success)

**Requirements:**
- Transparent background (or solid background is fine)
- Recommended size: 200-400px max dimension
- File format: GIF
- Keep the same filenames

**Where to find GIFs:**
- [GIPHY](https://giphy.com) - Search "couple animated", "romantic couple", "love animation"
- [Tenor](https://tenor.com) - Search "couple love animation"
- [LottieFiles](https://lottiefiles.com) - High-quality animated illustrations

### 3. Replace Sound Effects

Navigate to `assets/sounds/` and add your own sound files:

- `click-soft.mp3` - Continue button clicks (soft bloop/pop sound)
- `reveal.mp3` - Reveal interactions (gentle ding/chime)
- `no-escape.mp3` - NO button escaping (playful whoosh/boing) ~0.3s
- `screen-break.mp3` - Screen break effect (glass shatter) ~1-2s
- `yes-click.mp3` - YES button click (romantic chime)
- `success.mp3` - Success page (celebratory music) ~3-5s

**Requirements:**
- File format: MP3
- File size: <100KB each (optimized for web)
- Keep the same filenames

**Where to find sounds:**
- [Mixkit](https://mixkit.co/free-sound-effects/) - No attribution required
- [Freesound](https://freesound.org) - CC0 and CC-BY licenses
- [Pixabay](https://pixabay.com/sound-effects/) - Free, no attribution

### 4. Replace Screen Break Image

Navigate to `assets/images/` and replace:

- `screen-break.png` - The cracked screen overlay (1920x1080px recommended)

**Where to find:**
- Google Images: "broken screen overlay PNG transparent"
- Create your own using Canva or Photoshop

### 5. Add Instagram Photos (Optional)

Navigate to `assets/images/` and add profile images:

- `profile-1.jpg` - Circular cropped photo
- `profile-2.jpg` - Circular cropped photo
- `profile-3.jpg` - Heart-shaped cropped photo

To use them, add `<img>` tags in the success page section of `index.html`.

## 🚀 Deployment

### Option 1: GitHub Pages (Recommended - Free)

1. Commit and push all files to your `main` branch
2. Go to your repository **Settings**
3. Navigate to **Pages** section
4. Under **Source**, select:
   - Branch: `main`
   - Folder: `/ (root)`
5. Click **Save**
6. Your site will be live at: `https://[your-username].github.io/Myloveforyou`

### Option 2: Netlify (Fast & Easy)

1. Visit [app.netlify.com](https://app.netlify.com)
2. Drag and drop the entire `Myloveforyou` folder
3. Get instant deployment with custom URL
4. Optional: Set up custom domain

### Option 3: Vercel

1. Visit [vercel.com](https://vercel.com)
2. Import your GitHub repository
3. Framework preset: **Other**
4. Deploy - automatic builds on every push

## 🧪 Local Testing

Simply open `index.html` in any modern web browser:

- **Chrome** (recommended)
- **Firefox**
- **Safari**
- **Edge**

No build process or server required!

## 📱 Mobile Testing

The website is optimized for mobile devices. Test on:

- **iPhone SE** (320px - smallest screen)
- **iPhone 13/14** (390px)
- **Samsung Galaxy** (360px)
- **iPad** (768px)

Or use Chrome DevTools Device Mode (F12 → Toggle device toolbar).

## 🎨 Design Specifications

- **Colors**: Pink and red gradient theme (#FFB6C1, #FF69B4, #FF1493, #C71585)
- **Fonts**:
  - Headings: Pacifico (romantic script font)
  - Body: Quicksand (friendly rounded font)
- **Animation**: Smooth 15-second gradient flow background
- **Touch Targets**: Minimum 44x44px (mobile-friendly)
- **Responsive**: Works on screens from 320px to 1440px+

## 🔧 Technical Details

- **Tech Stack**: Pure HTML, CSS, JavaScript (no frameworks)
- **File Size**: ~50KB HTML + your assets
- **Browser Support**: All modern browsers (Chrome, Firefox, Safari, Edge)
- **Mobile Optimized**: Touch events, orientation support
- **Accessibility**: Reduced motion support, keyboard navigation

## 🎭 Special Features

### NO Button Behavior

The NO button has a special interactive mechanic:

1. **Hover/Click 1-7**: Button moves to random position on screen
2. **Attempt 8**: Triggers dramatic screen break effect with sound
3. **Screen Break**: Auto-dismisses after 6 seconds or when YES is clicked
4. **After Break**: NO button becomes permanently disabled

### Sound Effects

Sounds play on interactions but may be blocked on iOS Safari until first user interaction (this is normal browser behavior).

## 🐛 Troubleshooting

### Sounds don't play on iPhone

This is normal iOS behavior. Sounds will work after the first button click (Continue button on intro page).

### GIFs don't show

1. Check that GIF files are in `assets/gifs/` folder
2. Verify filenames match exactly (case-sensitive)
3. Ensure GIFs are uploaded to GitHub

### Screen break image doesn't show

1. Add `screen-break.png` to `assets/images/`
2. Use a PNG image with transparent or dark background
3. Recommended size: 1920x1080px

### NO button doesn't move on mobile

Try tapping the button directly. Movement is triggered by both hover (desktop) and touch (mobile).

## 💡 Tips for Best Experience

1. **Add all assets before sharing** - GIFs, sounds, and images enhance the experience
2. **Test on actual mobile device** - Emulators don't capture the full feel
3. **Write heartfelt messages** - Personal touches make it special
4. **Share the direct URL** - Send as a surprise link!

## 📄 License

This is a personal project. Feel free to customize and use for your own Valentine!

## ❤️ Credits

- **Fonts**: [Google Fonts](https://fonts.google.com) (Pacifico, Quicksand)
- **GIFs**: (Add your sources here)
- **Sounds**: (Add your sources here)

---

**Built with love 💕**

Share this link with your special someone and make Valentine's Day unforgettable!
