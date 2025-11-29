# @full-self-coding/core

Core library for automated code analysis and task execution.

## Installation

```bash
npm install @full-self-coding/core
```

## Usage

```javascript
import {
  analyzeCodebase,
  TaskSolverManager,
  createConfig,
  readConfigWithEnv,
  getGitRemoteUrls,
  CodeCommitter
} from '@full-self-coding/core';

// Create configuration
const config = createConfig({
  ai: {
    model: 'claude-sonnet',
    apiKey: 'your-api-key'
  }
});

// Analyze codebase
const tasks = await analyzeCodebase(config, gitUrl);

// Execute tasks
const taskSolver = new TaskSolverManager(config, gitUrl);
// ... execute tasks
```

## Features

- Code analysis engine
- Task execution framework
- Docker container management
- Code committing automation
- Configuration management
- Multiple AI model support

## License

MIT