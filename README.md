# Spotify MCP Bot - Complete Spotify Control Ecosystem

A comprehensive ecosystem for AI-powered Spotify control using the Model Context Protocol (MCP). This meta-project combines three specialized components to provide seamless Spotify integration through multiple interfaces.

## 🎵 What This Project Does

This ecosystem enables you to control Spotify playback and interact with your music library through Telegram bots backed by AI assistants.

## 🤖 Sample Use Cases
1. You can manage your Spotify playing session via the Telegram bot interface, leveraging advanced AI capabilities provided by the LLM controller to explore and discover new music based on user preferences.

2. If you have a shared Spotify player in your household, each family member can use the Telegram bot to control it remotely without needing physical access.

## 🏗️ Architecture Overview

```
┌─────────────────────┐    ┌──────────────────────┐    ┌─────────────────────┐
│   Telegram Bot      │    │   LLM Controller     │    │   MCP Server        │
│                     │    │                      │    │                     │
│ • User Interface    │◄──►│ • AI Integration     │◄──►│ • Spotify API       │
│ • Chat Commands     │    │ • Natural Language   │    │ • OAuth Handler     │
│ • Interactive Menus │    │ • Action Processing  │    │ • Playback Control  │
└─────────────────────┘    └──────────────────────┘    └─────────────────────┘
```

## 📦 Sub-Projects

### 1. [Spotify MCP Server](https://github.com/garywwh/spotify_mcp_server/)
**Core Spotify Integration**
- Direct Spotify Web API integration with OAuth2 authentication
- MCP-compliant server for standardized music control operations
- Handles playback, search, playlist management, and device control
- RESTful API endpoints for external integrations

### 2. [Spotify LLM Controller](https://github.com/garywwh/spotify_llm_controller/)
**AI-Powered Music Control**
- Bridges natural language commands to Spotify actions
- OpenAI integration for intelligent music recommendations
- Processes complex queries like "play something energetic for working out"
- Contextual understanding of music preferences and mood

### 3. [Spotify Telegram Bot](https://github.com/garywwh/spotify_telegram_bot/)
**User-Friendly Interface**
- Interactive Telegram bot for easy Spotify control
- Rich inline keyboards and command menus
- Real-time playback status and notifications
- Multi-user support with individual Spotify account linking


## Prerequisites
- Python 3.10 or higher
- Spotify Premium account (required for playback control)
- Spotify Developer App credentials
- OpenAI API key (for LLM features)
- Telegram Bot Token (for bot features)
## 🎯 Usage Examples

### Through Telegram Bot
```python
# Natural language commands
"Play some upbeat music for my morning run"
"Add this song to my favorites playlist"
"What's currently playing?"
"Skip to something more relaxing"
```

```python
# Direct commands
/play Taylor Swift
/pause
/skip
/playlist create "My Workout Mix"
/search artist "The Beatles"
```
