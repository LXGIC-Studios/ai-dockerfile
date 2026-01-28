# ai-dockerfile

Writing Dockerfiles is tedious. This tool scans your project and generates an optimized multi-stage Dockerfile that actually makes sense.

## Install

```bash
npm install -g ai-dockerfile
```

## Usage

```bash
# Generate a Dockerfile
npx ai-dockerfile

# Generate an optimized multi-stage build
npx ai-dockerfile --optimize

# Preview without writing
npx ai-dockerfile --preview

# Custom output path
npx ai-dockerfile --output ./docker/Dockerfile
```

## What it does

Looks at your project structure, figures out the runtime, framework, and build steps, then generates a proper multi-stage Dockerfile. It handles Node.js, Python, Go, Rust, and more.

## Requirements

Set your `OPENAI_API_KEY` environment variable.

```bash
export OPENAI_API_KEY=sk-...
```

## License

MIT
