# Elara

A Discord-like bot framework for building chat bots with commands, events, and interactions.

## Installation

```bash
pip install elara
```

## Quick Start

```python
from elara import Client

client = Client(token="your_token", prefix="!")

@client.command()
async def hello(ctx):
    await ctx.send("Hello, World!")

@client.on("message:new")
async def on_message(ctx):
    print(f"Message received: {ctx.content}")

await client.run()
```

## Features

- Command handling with prefix support
- Event listeners
- Cog system for organizing commands
- Built-in caching
- Rate limiting
- WebSocket connection management
- Embeds and components (buttons, action rows)

## License

MIT
