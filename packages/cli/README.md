# @full-self-coding/cli

CLI tool for automated code analysis and task execution.

## Installation

```bash
npm install -g @full-self-coding/cli
```

## Usage

```bash
# Run full analysis
full-self-coding

# Run with custom config
full-self-coding run --config ./my-config.json

# Show help
full-self-coding --help
```

## Commands

- `run` - Run the full self-coding analysis and task execution
- `--config <path>` - Specify custom configuration file
- `--help` - Show help information
- `--version` - Show version information

## Configuration

The CLI uses configuration from `~/.config/full-self-coding/config.json` by default. You can also specify environment variables:

- `FSC_AGENT_TYPE` - AI agent type
- `FSC_ANTHROPIC_API_KEY` - Anthropic API key
- `FSC_GOOGLE_GEMINI_API_KEY` - Google Gemini API key

## Examples

```bash
# Basic usage
full-self-coding

# With custom config
full-self-coding run --config ./project-config.json

# Using environment variables
export FSC_ANTHROPIC_API_KEY="your-key"
full-self-coding
```

## License

MIT