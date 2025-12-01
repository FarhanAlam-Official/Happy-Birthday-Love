## 🎉 Birthday Website Template for Your Love ❤️

A beautiful, interactive, and personalized birthday website built with Next.js, React, and Framer Motion. This website features multiple interactive sections including photo galleries, games, quizzes, and a special cake finale with fireworks animations.

Perfect for creating a memorable birthday surprise for someone you deeply love!

## 🎁 What Makes This Special?

This is a **fully customizable template** that you can personalize for your best friend's birthday. Simply add your photos, customize the messages, and deploy!

📖 **[Complete Setup Guide](SETUP.md)** - Step-by-step instructions to customize this template

## ✨ Features

### 🎨 Interactive Sections

- **Hero Section** - Animated welcome with personalized messages
- **Love Letter** - Revealing letter with smooth animations
- **Photo Gallery** - Categorized photo collections (funny, emotional, trips, chaos)
- **Secret Vault** - Password-protected gallery with special memories
- **3D Memory Ring** - Interactive 3D carousel of all memories
- **Balloon Pop Game** - Interactive game with hidden messages
- **Love Timeline** - Chronological journey of your story together
- **Flip Cards** - Reasons why they're your soulmate
- **Love Quiz** - Fun quiz to test how well they know you
- **Cake Finale** - Interactive cake with candles, wishes, and fireworks

### 🎭 Visual Effects

- Floating balloons and hearts
- Particle background animations
- Confetti effects
- Fireworks animations (after blowing candles)
- Smooth page transitions
- 3D image rotations
- Image protection (right-click and drag disabled)

### 🎨 Design

- Red/pink love theme (fully customizable)
- Responsive design (mobile-friendly)
- Modern UI with glassmorphism effects
- Smooth animations using Framer Motion
- Beautiful gradients and shadows

## 🛠️ Tech Stack

- **Framework**: Next.js 16
- **React**: 19.2.0
- **TypeScript**: 5.x
- **Styling**: Tailwind CSS 4.x
- **Animations**: Framer Motion
- **UI Components**: Radix UI
- **Icons**: Lucide React

## 🚀 Getting Started

### Prerequisites

- Node.js 18+ (or use pnpm/npm)
- pnpm (recommended) or npm/yarn

### Installation

1. **Clone the repository**

   ```bash
   git clone <repository-url>
   cd birthday-website-template
   ```

2. **Install dependencies**

   ```bash
   pnpm install
   # or
   npm install
   ```

3. **Customize the configuration**

   Edit `lib/config.ts` to personalize:
   - Names (her name, your name, nickname)
   - Secret vault password
   - Photo paths
   - Messages and text content
   - Quiz questions
   - Timeline events
   - And more!

4. **Add your images**

   Place your images in the `public/images/` folder following this structure:
   - `public/images/hero/` - Hero section images (13+ photos)
   - `public/images/gallery/funny/` - Funny moments
   - `public/images/gallery/emotional/` - Emotional moments
   - `public/images/gallery/trips/` - Travel & adventures
   - `public/images/gallery/chaos/` - Chaotic moments
   - `public/images/timeline/` - Timeline event images
   - `public/images/secret/` - Password-protected images
   - `public/images/birthday-card.jpg` - Birthday card image
   - `public/images/birthday-video.mp4` - Optional video message

   📖 See `public/images/README.md` for detailed image setup instructions.

   Then update the paths in `lib/config.ts` to match your images.

5. **Run the development server**

   ```bash
   pnpm dev
   # or
   npm run dev
   ```

6. **Open your browser**

   Navigate to [http://localhost:3000](http://localhost:3000)

## 📁 Project Structure

```bash
birthday-website-template/
├── app/
│   ├── globals.css          # Global styles
│   ├── layout.tsx           # Root layout
│   └── page.tsx             # Main page component
├── components/
│   ├── ui/                  # Reusable UI components (Radix UI)
│   ├── 3d-image-ring.tsx   # 3D memory ring component
│   ├── balloon-game.tsx    # Balloon pop game
│   ├── bestie-quiz.tsx     # Friendship quiz
│   ├── cake-finale.tsx     # Cake with candles and fireworks
│   ├── confetti-effect.tsx # Confetti animation
│   ├── flip-cards.tsx      # Soulmate reasons cards
│   ├── floating-balloons.tsx # Floating balloon animation
│   ├── friendship-timeline.tsx # Timeline component
│   ├── hero-section.tsx    # Hero section
│   ├── love-letter.tsx     # Love letter component
│   ├── particles-background.tsx # Particle background
│   ├── photo-gallery.tsx  # Photo gallery
│   └── secret-vault-modal.tsx # Secret vault modal
├── lib/
│   ├── config.ts           # ⭐ MAIN CONFIGURATION FILE
│   └── utils.ts            # Utility functions
├── public/                 # Static assets (images, etc.)
├── hooks/                  # Custom React hooks
└── styles/                 # Additional styles
```

## 🎨 Customization Guide

### Main Configuration (`lib/config.ts`)

This is the **most important file** for personalization. Edit it to customize:

#### 1. **Names & Personalization**

```typescript
herName: "Your Love",     // Birthday person's name
nickname: "My Love",      // Their nickname
yourName: "Your Name",    // Your name
```

#### 2. **Secret Vault Password**

```typescript
magicCode: "easypass",    // Change to your secret code
```

#### 3. **Photos**

- Add your photos to the `public/` folder
- Update the paths in:
  - `publicGalleries` (funny, emotional, trips, chaos)
  - `secretGallery`
  - `timelineEvents[].image`
  - `birthdayCardImage`

#### 4. **Content**

- `letterText`: Love letter paragraphs
- `balloonMessages`: Messages inside balloons
- `soulmateReasons`: Reasons on flip cards
- `quizQuestions`: Quiz questions and answers
- `timelineEvents`: Your friendship timeline

#### 5. **Video Message**

```typescript
finalVideoUrl: "https://www.youtube.com/embed/YOUR_VIDEO_ID"
```

### Styling

The theme uses a red/pink love palette. To change the color scheme:

1. Edit `app/globals.css` for global color variables
2. Update Tailwind classes in components
3. Modify gradients in `lib/config.ts`

## 🚢 Deployment

### Vercel (Recommended)

1. Push your code to GitHub
2. Import your repository on [Vercel](https://vercel.com)
3. Vercel will automatically detect Next.js and deploy

### Other Platforms

Build the project:

```bash
pnpm build
# or
npm run build
```

The output will be in the `.next` folder. Deploy this to any static hosting service.

## 📝 Available Scripts

- `pnpm dev` - Start development server
- `pnpm build` - Build for production
- `pnpm start` - Start production server
- `pnpm lint` - Run ESLint

## 🎯 Features Breakdown

### Cake Finale Section

- Interactive cake with 5 candles
- Wish-making sequence with animated phrases
- Candle blowing animation
- Fireworks display after blowing candles
- Flip card with birthday message
- Optional video message embed

### Photo Gallery

- Categorized galleries (funny, emotional, trips, chaos)
- Lightbox view for images
- Secret vault access button
- Image protection (right-click disabled)

### 3D Memory Ring

- Interactive 3D carousel
- Draggable rotation
- Hover effects
- All memories in one place

### Balloon Game

- 15 interactive balloons
- Hidden messages inside
- Pop animation
- Progress tracking

## 🔒 Image Protection

Images are protected from:

- Right-click context menu
- Drag and drop
- Direct URL access (if deployed with proper server config)

## 💡 Tips

1. **Image Optimization**: Use optimized images (WebP format recommended)
2. **Video Embed**: Use YouTube/Vimeo embed URLs for the final video
3. **Testing**: Test on mobile devices for responsive design
4. **Performance**: Images are lazy-loaded for better performance

## 🐛 Troubleshooting

### Images not showing?

- Check file paths in `lib/config.ts`
- Ensure images are in the `public/` folder
- Verify file names match exactly (case-sensitive)

### Build errors?

- Clear `.next` folder: `rm -rf .next`
- Reinstall dependencies: `rm -rf node_modules && pnpm install`
- Check Node.js version (18+ required)

### Animations not working?

- Ensure JavaScript is enabled
- Check browser console for errors
- Verify Framer Motion is installed

## ❤️ Made with Love

This is an open-source template created to help you make romantic, memorable birthday celebrations. Customize it, make it yours, and share the joy!

---

## 🤝 Contributing

Feel free to submit issues and enhancement requests!

## 📜 License

MIT License - feel free to use this template for personal projects.
