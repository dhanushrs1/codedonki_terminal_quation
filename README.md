# 🎮 CodeDonki - Interactive AR Coding Learning Platform

<div align="center">

![CodeDonki](uploads/codedonki-logo.svg)

**Play, Learn, Code & Laugh!**

*An immersive, gamified coding education platform with AR integration, interactive lessons, and coding games designed for young learners.*

[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/)
[![Flask](https://img.shields.io/badge/Flask-3.1.2-green.svg)](https://flask.palletsprojects.com/)
[![SQLite](https://img.shields.io/badge/SQLite-3-lightgrey.svg)](https://www.sqlite.org/)
[![License](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

[🚀 Quick Start](#-quick-start) • [📚 Documentation](#-table-of-contents) • [🎮 Features](#-features) • [🛠 Development](#-development-guide)

</div>

---

## 📋 Table of Contents

1. [Overview](#-overview)
2. [Features](#-features)
3. [Tech Stack](#-tech-stack)
4. [Prerequisites](#-prerequisites)
5. [Quick Start](#-quick-start)
6. [Detailed Installation](#-detailed-installation)
7. [Configuration](#-configuration)
8. [Database Setup](#-database-setup)
9. [Running the Application](#-running-the-application)
10. [Project Structure](#-project-structure)
11. [Development Guide](#-development-guide)
12. [API Documentation](#-api-documentation)
13. [Deployment](#-deployment)
14. [Troubleshooting](#-troubleshooting)
15. [Contributing](#-contributing)
16. [License](#-license)

---

## 🌟 Overview

**CodeDonki** is a comprehensive, gamified learning platform that makes coding education fun and interactive for young learners. Built with Flask and SQLite, it combines traditional lessons with modern AR (Augmented Reality) experiences, interactive quizzes, and engaging coding games.

### What Makes CodeDonki Special?

- 🎯 **Hands-On Learning**: Interactive lessons with AR model integration
- 🎮 **Gamified Experience**: XP points, badges, and leaderboards
- 🧠 **Coding Games**: Three interactive games to reinforce learning
- 🤖 **AI-Powered**: Personalized learning suggestions via Google Gemini
- 📊 **Progress Tracking**: Detailed analytics and achievement system
- 👨‍💼 **Full Admin Panel**: Complete content management system
- 📱 **Responsive Design**: Works perfectly on all devices

---

## ✨ Features

### 🎓 Learning System

#### Interactive Lessons
- **AR-Enhanced Content**: Lessons with 3D AR models for immersive learning
- **Category Organization**: Lessons grouped by topics (Python, Web Dev, Data Science, etc.)
- **Progressive Unlocking**: Complete lessons to unlock the next ones
- **Rich Content**: HTML-based lessons with embedded code examples
- **Slug-Based URLs**: SEO-friendly lesson URLs

#### Quiz System
- **Multiple Choice Questions**: 4-option quizzes with explanations
- **Automatic Grading**: Instant feedback on quiz submissions
- **Pass Threshold**: Configurable passing scores (default: 70%)
- **XP Rewards**: Variable XP based on performance (min-max range)
- **Retry Capability**: Retake quizzes until you pass
- **Progress Tracking**: View all quiz attempts and scores

#### Lesson Progress
- **Completion Tracking**: Mark lessons as completed
- **Unlock System**: Next lesson unlocks when you pass the current quiz
- **XP Accumulation**: Earn experience points for completing lessons
- **Badge Achievements**: Unlock badges at XP milestones

### 🎮 Gamification Features

#### Three Interactive Coding Games

**1. 🧠 Code Memory Game (Beginner - 15 XP)**
- Match Python code snippets with their outputs
- 8 pairs of cards (16 total)
- Tracks moves and completion time
- Teaches: Print statements, operators, string manipulation, boolean logic

**2. ⌨️ Code Typing Race (Intermediate - 25 XP)**
- Speed typing challenge with real Python code
- 60-second timer
- Real-time WPM (Words Per Minute) calculation
- Accuracy tracking
- 5 different code snippets including loops, functions, and data structures

**3. 🧩 Code Puzzle (Advanced - 30 XP)**
- Solve 8 Python programming challenges
- Write actual Python functions
- Progressive difficulty
- Hints provided for each puzzle
- Covers: Basic math, conditionals, loops, string operations, recursion

#### Leaderboard System
- **Global Rankings**: Top 50 users by XP
- **User Profiles**: Display avatars and names
- **Real-Time Updates**: See your rank climb as you earn XP
- **Competitive Learning**: Motivates users to complete more lessons

#### Badge System
- **Achievement Badges**: Unlock badges at XP thresholds
- **8 Default Badges**: From "Getting Started" (10 XP) to "Coding Legend" (1000 XP)
- **Custom Badges**: Admins can create custom achievement badges
- **Profile Display**: Show earned badges on your profile
- **Auto-Award**: Badges automatically awarded when XP threshold reached

### 🤖 AI-Powered Features

- **Gemini AI Integration**: Powered by Google's Generative AI
- **Contextual Learning Tips**: Get personalized tips after completing lessons
- **Smart Suggestions**: AI analyzes lesson content and provides relevant advice
- **Fallback System**: Graceful degradation if AI is unavailable

### 👨‍💼 Admin Panel

#### Dashboard
- **Real-Time Statistics**: Total users, lessons, categories, quiz questions
- **Recent Activity**: User registrations, lesson completions, badge earnings
- **Analytics Charts**: User activity, completion rates, category distribution
- **Quick Actions**: Jump to any management section

#### User Management
- **View All Users**: See all registered users with stats
- **Promote to Admin**: Elevate users to admin role
- **Reset Progress**: Clear user's XP, lessons, and badges
- **Delete Users**: Remove users and all associated data
- **Award Badges**: Manually award missing badges based on XP

#### Lesson Management
- **CRUD Operations**: Create, Read, Update, Delete lessons
- **AR Code Upload**: Paste HTML/AR code or upload files
- **Category Assignment**: Organize lessons into categories
- **Ordering**: Set lesson order within categories
- **XP Configuration**: Set min/max XP rewards
- **Pass Threshold**: Configure quiz passing percentage
- **Slug Management**: Auto-generated SEO-friendly URLs

#### Category Management
- **Create Categories**: Add new learning topics
- **Visual Customization**: Set colors and icons for each category
- **SEO Optimization**: Custom slugs and meta descriptions
- **Lesson Count**: See how many lessons in each category

#### Quiz Management
- **Question Creation**: Add quiz questions for any lesson
- **Four Options**: A, B, C, D answer choices
- **Correct Answer**: Mark the right answer
- **Explanations**: Provide detailed explanations for learning
- **Bulk Management**: View and edit all questions for a lesson

#### Badge Management
- **Create Badges**: Define achievement badges
- **XP Thresholds**: Set when badges are earned
- **Visual Design**: Choose colors and icons
- **Active/Inactive**: Enable or disable badges
- **Unique Names**: Ensure badge names are unique

### 🎨 UI/UX Features

- **Modern Design**: Gradient-based, colorful interface
- **CodeDonki Theme**: Consistent branding with sky blue, orange, lime green, purple
- **Smooth Animations**: CSS transitions and hover effects
- **Responsive Layout**: Mobile-first design, works on all screen sizes
- **Font Awesome Icons**: Professional icon library
- **Modal Interfaces**: Clean, focused game and quiz experiences
- **Toast Notifications**: User-friendly success/error messages

---

## 🛠 Tech Stack

### Backend

| Technology | Version | Purpose |
|-----------|---------|---------|
| **Python** | 3.8+ | Core programming language |
| **Flask** | 3.1.2 | Web framework and API |
| **SQLite** | 3 | Serverless database |
| **PyJWT** | 2.10.1 | JWT token authentication |
| **Passlib** | 1.7.4 | Password hashing (PBKDF2) |
| **Google Generative AI** | 0.8.5 | AI-powered suggestions |
| **Python-dotenv** | 1.1.1 | Environment configuration |
| **Flask-CORS** | 6.0.1 | Cross-origin resource sharing |

### Frontend

| Technology | Purpose |
|-----------|---------|
| **HTML5** | Structure and semantics |
| **CSS3** | Styling with gradients and animations |
| **Vanilla JavaScript** | Client-side interactivity |
| **Jinja2** | Server-side templating |
| **Font Awesome** | Icon library |

### Database Schema

- **users**: User accounts and profiles
- **categories**: Learning topic categories
- **lessons**: Course lessons with AR content
- **quiz_questions**: Multiple-choice questions
- **lesson_progress**: User progress tracking
- **user_quiz_attempts**: Quiz attempt history
- **badges**: Achievement badges
- **user_badges**: Junction table for earned badges

---

## 📦 Prerequisites

Before installing CodeDonki, ensure you have:

- ✅ **Python 3.8 or higher** (Python 3.10+ recommended)
- ✅ **pip** (Python package manager)
- ✅ **Virtual environment** support (venv)
- ✅ **Modern web browser** (Chrome, Firefox, Safari, Edge)
- ✅ **Google Gemini API Key** (free from Google AI Studio)
- ✅ **Git** (for cloning the repository)

### System Requirements

- **OS**: Windows 10+, macOS 10.14+, or Linux
- **RAM**: 2GB minimum (4GB recommended)
- **Storage**: 500MB free space
- **Internet**: Required for AI features

---

## 🚀 Quick Start

Get CodeDonki running in 5 minutes:

```bash
# 1. Clone the repository
git clone https://github.com/yourusername/codedonki.git
cd codedonki

# 2. Create and activate virtual environment
python -m venv venv
# Windows:
venv\Scripts\activate
# macOS/Linux:
source venv/bin/activate

# 3. Install dependencies
pip install -r requirements.txt

# 4. Create environment file
cp env_template.txt .env
# Edit .env and add your API keys

# 5. Create admin user
python create_admin.py

# 6. Run the application
python app.py
```

**🎉 Done!** Visit http://127.0.0.1:5000

---

## 📥 Detailed Installation

### Step 1: Clone the Repository

```bash
git clone https://github.com/yourusername/codedonki.git
cd codedonki
```

Or download the ZIP file and extract it.

### Step 2: Create Virtual Environment

**Windows:**
```bash
python -m venv venv
venv\Scripts\activate
```

**macOS/Linux:**
```bash
python3 -m venv venv
source venv/bin/activate
```

You should see `(venv)` in your terminal prompt.

### Step 3: Install Dependencies

```bash
pip install -r requirements.txt
```

This installs all required packages:
- Flask and extensions
- Authentication libraries
- Google Generative AI
- Database conn
