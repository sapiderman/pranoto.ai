# Pranoto.ai

## Prerequisities

- [Docker](https://www.docker.com/) v20.x.x
- [Docker compose](https://docs.docker.com/compose/) v2
- [Node.js](https://nodejs.org/en) v16.x.x
- [FFmpeg](https://ffmpeg.org/) v6.0
- [Python](https://www.python.org/) v3.9.9
- [Whisper](https://github.com/openai/whisper) v20230314

## Getting Started

1. Run the system dependencies

```sh
cd .dev && docker compose up -d && cd ..
```

2. Run the frontend dependencies

````sh
cd frontend
npm ci
```

3. Run the worker:

```sh
npm run worker
````

4. Run the development server:

```sh
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

## API Demo Usage

Use CURL, Postman, or run the API url in browser:

[http://localhost:3000/api/upload-example](http://localhost:3000/api/upload-example)

Wait for some time and check again to see the result file in `public/audios/audio.mp3` and `public/texts/audio.json`
