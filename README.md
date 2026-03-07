# Mattermost CLI Skill

Fetch and display Mattermost messages using the mm CLI or direct API calls.

## Installation

### For Clawdbot

```bash
clawdhub install mattermost-cli
```

### From GitHub

```bash
git clone https://github.com/ThneAI/mattermost-cli-skill.git
cd mattermost-cli-skill
```

## Usage

Once installed, the skill will automatically trigger when you ask about Mattermost messages.

### Example Queries

- "Check my recent Mattermost messages"
- "What did Alice say about the deployment?"
- "Find any tasks from my chat with Bob"
- "Show me my DMs from the last 24 hours"

## Prerequisites

You need to have Mattermost CLI (`mm`) installed and configured:

```bash
# Install mm CLI
npm install -g mattermost-cli

# Configure
mm config --init
```

Or set environment variables:

```bash
export MM_URL="http://your-mattermost.com"
export MM_TOKEN="your-personal-access-token"
```

## Features

- ✅ Fetch DM messages
- ✅ Filter by user
- ✅ Filter by time range
- ✅ List channels
- ✅ JSON output for parsing
- ✅ Automatic secret redaction

## Security

All output is automatically redacted for safe LLM processing:
- API keys
- Tokens
- Passwords
- Connection strings

## License

MIT
