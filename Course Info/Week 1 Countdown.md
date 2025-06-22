# Week 1 - Countdown Timer PRD

## Product Requirements Document: Static Retirement Countdown Timer

### 🎯 Overview
Build a modern, responsive React.js countdown timer that displays the time remaining until retirement (Aug 12, 2033 @ 12:00 PM). This will serve as the foundation for the earlyexit.fun application.

---

## 📋 Requirements

### Functional Requirements
- **Primary Display**: Show countdown to retirement date in real-time
- **Time Units**: Display years, months, days, hours, minutes, and seconds
- **Configuration**: Retirement date/time should be configurable via config file
- **Real-time Updates**: Timer updates every second
- **Responsive Design**: Works seamlessly on desktop, tablet, and mobile

### Non-Functional Requirements
- **Performance**: Smooth animations, no flickering
- **Accessibility**: Screen reader friendly, proper color contrast
- **Browser Support**: Modern browsers (Chrome, Firefox, Safari, Edge)
- **Mobile-First**: Optimized for mobile viewing experience

---

## 🎨 Design Specifications

### Visual Design
- **Theme**: Modern, clean, financial/investment aesthetic
- **Color Palette**: 
  - Primary: Deep blue (#1e3a8a)
  - Secondary: Green (#10b981) for positive numbers
  - Background: Light gray (#f8fafc)
  - Text: Dark gray (#1f2937)
- **Typography**: Clean, readable fonts (Inter or similar)
- **Layout**: Centered design with responsive grid for time units

### Mobile Considerations
- **Breakpoints**: 
  - Mobile: < 768px
  - Tablet: 768px - 1024px
  - Desktop: > 1024px
- **Touch-Friendly**: Adequate spacing for touch interactions
- **Readable Text**: Minimum 16px font size on mobile

---

## 🏗️ Technical Architecture

### Project Structure
```
earlyexit.fun/
├── README.md
├── .gitignore
├── package.json
├── public/
│   ├── index.html
│   └── favicon.ico
├── src/
│   ├── components/
│   │   ├── CountdownTimer.jsx
│   │   └── TimeUnit.jsx
│   ├── config/
│   │   └── retirement-config.js
│   ├── styles/
│   │   ├── App.css
│   │   └── CountdownTimer.css
│   ├── utils/
│   │   └── timeCalculations.js
│   ├── App.jsx
│   └── index.js
└── backend/ (placeholder for future weeks)
```

### Technology Stack
- **Frontend Framework**: React.js 18+
- **Build Tool**: Vite (faster than Create React App)
- **Styling**: CSS3 with Flexbox/Grid
- **State Management**: React hooks (useState, useEffect)
- **Package Manager**: npm

---

## 🛠️ Implementation Plan

### Phase 1: Environment Setup (30 minutes)
1. **Install Prerequisites**
   - Node.js (v18 or higher)
   - Git
   - Cursor IDE setup

2. **Project Initialization**
   - Create project folder structure
   - Initialize React with Vite
   - Set up Git repository
   - Install necessary dependencies

### Phase 2: Core Component Development (2 hours)
1. **Configuration Setup**
   - Create retirement-config.js
   - Define retirement date and timezone

2. **Utility Functions**
   - Time calculation logic
   - Date formatting helpers

3. **React Components**
   - CountdownTimer (main component)
   - TimeUnit (reusable component for each time segment)

### Phase 3: Styling & Responsiveness (1.5 hours)
1. **CSS Implementation**
   - Mobile-first responsive design
   - Modern visual styling
   - Smooth animations/transitions

2. **Testing & Refinement**
   - Cross-device testing
   - Performance optimization

---

## 📱 Component Specifications

### CountdownTimer Component
```jsx
// Main countdown display component
- Manages timer state and updates
- Calculates time differences
- Renders grid of TimeUnit components
- Handles responsive layout
```

### TimeUnit Component
```jsx
// Individual time segment (years, months, etc.)
- Props: value, label, size
- Displays number and label
- Responsive styling based on screen size
```

### Configuration File
```javascript
// retirement-config.js
- Retirement date: August 12, 2033 12:00 PM
- Timezone handling
- Display preferences
- Future: user customization options
```

---

## 🎯 Success Criteria

### MVP Completion Checklist
- [ ] React app runs locally without errors
- [ ] Countdown displays accurate time remaining
- [ ] Timer updates every second smoothly
- [ ] Responsive design works on mobile/desktop
- [ ] Modern, professional appearance
- [ ] Retirement date configurable via config file
- [ ] Code is clean and well-organized
- [ ] Git workflow established

### Performance Targets
- **Load Time**: < 2 seconds on 3G connection
- **Frame Rate**: 60fps animations
- **Bundle Size**: < 500KB initial load

---

## 🚀 Getting Started

### Step 1: Mac Development Environment Setup

#### Install Prerequisites
```bash
# Install Homebrew (if not already installed)
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"

# Install Node.js (includes npm)
brew install node

# Verify installation
node --version  # Should be v18 or higher
npm --version
```

#### Install Git (if not already installed)
```bash
# Check if git is installed
git --version

# If not installed:
brew install git

# Configure git (replace with your info)
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"
```

### Step 2: Project Setup

#### Create Project Directory
```bash
# Navigate to your development folder
cd ~/Documents  # or wherever you keep projects

# Create and enter project directory
mkdir earlyexit.fun
cd earlyexit.fun

# Initialize React project with Vite
npm create vite@latest . -- --template react

# Install dependencies
npm install

# Test that everything works
npm run dev
```

#### Set Up Git Repository
```bash
# Initialize git (if not already done by Vite)
git init

# Add initial files
git add .
git commit -m "Initial React project setup"

# Connect to GitHub (create the repo on GitHub first)
git remote add origin https://github.com/yourusername/earlyexit.fun.git
git push -u origin main
```

### Step 3: Project Structure Setup

#### Create Additional Directories
```bash
# Create additional folders for organization
mkdir src/components src/config src/styles src/utils

# Create placeholder files
touch src/components/CountdownTimer.jsx
touch src/components/TimeUnit.jsx
touch src/config/retirement-config.js
touch src/utils/timeCalculations.js
touch src/styles/CountdownTimer.css
```

### Step 4: Install Additional Dependencies
```bash
# Install any additional packages we might need
npm install --save-dev @types/react @types/react-dom
```

---

## 📝 Next Steps After Completion

1. **Test thoroughly** on different devices and browsers
2. **Optimize performance** - check for memory leaks or excessive re-renders
3. **Document the code** - add comments and update README
4. **Prepare for Week 2** - this static timer will become the foundation for the authenticated React app

---

## 🐛 Common Issues & Solutions

### Node.js Version Issues
- **Problem**: Older Node.js version causing build errors
- **Solution**: Use `nvm` to manage Node versions or update via Homebrew

### Port Already in Use
- **Problem**: `npm run dev` fails because port 5173 is busy
- **Solution**: Kill the process or use `npm run dev -- --port 3000`

### Git Push Issues
- **Problem**: Permission denied when pushing to GitHub
- **Solution**: Set up SSH keys or use GitHub CLI

---

## 📚 Learning Resources

- [React Official Tutorial](https://react.dev/learn)
- [Vite Documentation](https://vitejs.dev/guide/)
- [CSS Grid Guide](https://css-tricks.com/snippets/css/complete-guide-grid/)
- [Responsive Design Basics](https://web.dev/responsive-web-design-basics/)

---

*Ready to build your first React countdown timer? Let's get started with the environment setup!*