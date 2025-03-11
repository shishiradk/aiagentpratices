# Event Checking AI Agent

## Overview
Event Checking AI Agent is an automated system built using **n8n** that integrates with Google Calendar and an AI model to check for upcoming events. When a chat message is received, it retrieves events from Google Calendar and processes them using an AI Agent powered by DeepSeek and OpenAI models to provide relevant responses.

## Features
- Listens for chat messages to trigger event checking.
- Fetches upcoming events from Google Calendar.
- Uses an AI Agent to process and interpret event data.
- Leverages OpenAI's LLM for advanced text-based interaction.

## Tech Stack
- **n8n** (Workflow automation)
- **Google Calendar API** (For event retrieval)
- **DeepSeek LLM (8B model)** (AI-based processing)
- **OpenAI API** (For chat-based AI interactions)

## Installation
1. Clone the repository:
   ```sh
   git clone https://github.com/your-username/event-checking-ai-agent.git
   cd event-checking-ai-agent
   ```
2. Install and configure **n8n**:
   ```sh
   npm install -g n8n
   n8n start
   ```
3. Set up credentials:
   - Connect Google Calendar via OAuth.
   - Add OpenAI API credentials.
4. Import the provided **n8n** workflow JSON file.

## Usage
- Ensure that **n8n** is running.
- Send a chat message to trigger the AI agent.
- The system will fetch events from Google Calendar and provide responses.
- AI will process and respond accordingly based on event data.

## Workflow Structure
1. **Chat Trigger** - Detects incoming messages.
2. **Google Calendar Integration** - Fetches up to 5 upcoming events.
3. **AI Agent Processing** - Parses event data and generates relevant output.
4. **OpenAI Chat Model** - Enhances response quality using LLM.

## Future Improvements
- Add support for multiple calendar accounts.
- Enhance AI response capabilities with additional prompt tuning.
- Implement voice command support.

## License
This project is open-source. Feel free to use and modify it as needed.

