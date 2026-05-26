# AI Fitness Trainer

A modern, full-stack AI fitness application that combines a multi-layered neural network recommendation engine, real-time pose tracking, Retrieval-Augmented Generation (RAG), and live API integrations to provide truly adaptive, personalised workout and diet plans.
<p align="center">
  <img src="screenshots/banner.png" width="100%" alt="AI Fitness Trainer Banner">
</p>

<h1 align="center">🏋️ AI Fitness Trainer</h1>

<p align="center">
An intelligent full-stack fitness platform powered by Artificial Intelligence, Deep Learning, Computer Vision, and Retrieval-Augmented Generation (RAG).
</p>

<p align="center">
  <img src="https://img.shields.io/badge/FastAPI-Backend-green">
  <img src="https://img.shields.io/badge/PyTorch-DeepLearning-red">
  <img src="https://img.shields.io/badge/MediaPipe-PoseTracking-blue">
  <img src="https://img.shields.io/badge/Gemini-AI-orange">
  <img src="https://img.shields.io/badge/SQLite-Database-lightgrey">
  <img src="https://img.shields.io/badge/License-MIT-yellow">
</p>

---

# 📖 Overview

AI Fitness Trainer is a modern AI-powered fitness ecosystem that combines Deep Learning, Retrieval-Augmented Generation (RAG), Machine Learning, and real-time pose estimation to deliver adaptive workout and nutrition recommendations.

Built using FastAPI, PyTorch, MediaPipe, Gemini AI, and scikit-learn, the platform provides:

- 🧠 Intelligent workout generation
- 🍽️ Personalized diet planning
- 📷 Real-time exercise coaching
- 📊 Advanced analytics tracking
- 🏆 Gamified fitness challenges
- 🔊 Live voice feedback
- 💪 Progressive overload recommendations

The system is designed with a layered AI architecture that remains functional even when external APIs fail, making it robust, scalable, and production-inspired.

---

# ✨ Core Features

## 🧠 AI Recommendation System

- Gemini-powered personalized workout and diet generation
- TF-IDF Retrieval-Augmented Generation (RAG) pipeline
- Hallucination prevention using curated exercise retrieval
- Context-aware workout planning
- Equipment-aware recommendations
- Goal-based adaptive training

---

## 🤖 Deep Learning Fallback Engine

- Custom PyTorch Seq2Seq Encoder-Decoder model
- Generates workout sequences locally
- Automatically activates when Gemini API fails
- Trained on categorized exercise datasets
- Fully offline-capable fallback recommendation system

---

## 📷 Real-Time Live AI Coach

- MediaPipe Pose-based exercise tracking
- Real-time rep counting
- Joint-angle calculations
- Form correction warnings
- Webcam-based posture analysis
- Live alignment monitoring

Supported exercises include:

1. Squats
2. Lunges
3. Push-ups
4. Shoulder Press
5. Plank

---

## 🔊 Audio Fitness Coach

- Real-time spoken feedback
- Rep milestone announcements
- Exercise correction voice prompts
- Hands-free workout experience

---

## 🍽️ Smart Nutrition Engine

- Live Edamam Recipe API integration
- Personalized meal plans
- Accurate macro calculations
- Real food images and recipes
- Calorie tracking
- Food logging system

---

## 📊 Advanced Analytics

- Workout history tracking
- Calorie burn charts
- 1RM (One Rep Max) progression tracking
- Weekly performance visualization
- ML-generated Fitness Score predictions

---

## 🏆 Gamification System

- Daily streak tracking
- Fitness badges
- Built-in workout challenges
- Achievement system
- Motivation-based progression

---

## 🔐 Security Features

- JWT authentication
- Bcrypt password hashing
- Secure API endpoints
- Protected user sessions

---

## 🎨 Modern UI/UX

- Glassmorphic dashboard
- Bento-grid layouts
- Smooth animations
- Fully responsive design
- Dark-mode aesthetic
- Interactive workout cards

---

# 🚀 What Makes This Project Unique?

Unlike traditional fitness applications that rely on static workout templates, AI Fitness Trainer uses a layered AI architecture:

- Retrieval-Augmented Generation (RAG) ensures recommendations remain grounded in curated exercise knowledge.
- A custom PyTorch Seq2Seq model acts as a local AI fallback system.
- Database-level API caching minimizes token usage and improves scalability.
- MediaPipe enables real-time computer vision-based coaching directly in the browser.
- Machine Learning models predict personalized Fitness Scores using historical user data.

This creates a resilient, production-inspired AI system rather than a simple CRUD-based fitness tracker.

---

# 🏗️ System Architecture

```text
User Request
     │
     ▼
Database Cache Check
     │
 ┌── Yes ──► Return Cached Result
 │
 No
 │
 ▼
RAG Retrieval Engine
 │
 ▼
Gemini AI Recommendation
 │
API Failure?
 │
 ├── No ──► Save to Cache ──► Return Result
 │
 └── Yes
        │
        ▼
PyTorch Seq2Seq Model
        │
        ▼
Save to Cache ──► Return Result
```