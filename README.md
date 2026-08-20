# Ambient Insight Stream

Front-End UI Layout & Device Permissions: "Write a clean, responsive HTML5, CSS3, and JavaScript front-end page for an ambient AI assistant app. The interface must include a control panel with toggle buttons to 'Enable Spatial Sensors' (Camera and Microphone access) and a dynamic grid of user interest tags (e.g., 'Architecture', 'Nature', 'Translation', 'Safety Hazards'). Include a video preview element to show the live camera feed and a clean scrolling logs panel titled 'Ambient Insight Stream' where system logs and AI-generated data cards will appear."

Media Capturing & Frame Slicing Logic: "Write the client-side JavaScript code to securely request camera and microphone permissions via navigator.mediaDevices.getUserMedia. Once active, implement a loop function using an HTML5 <canvas> element that silently grabs a compressed JPEG snapshot of the video frame every 3 seconds. Package this image frame and a brief audio array snippet into a payload ready to be sent to a back-end server via a Fetch POST request or a WebSocket message." Back-End Processing API with Multimodal Integration: "Create a Python FastAPI back-end endpoint /api/spatial-process that accepts an image file, an audio file, and an array of user preferences. Integrate this endpoint with a multimodal LLM API. The prompt to the AI model should say: 'You are an ambient spatial assistant. Analyze this image frame and environmental sound. Filter your observations strictly against the user's selected interests: {user_interests}. If anything relevant is found, return a punchy, 1-sentence contextual insight. If nothing matches, return an empty string.' Return this data instantly back to the client UI."

This project was built with [Lovable](https://lovable.dev).

## Build with Lovable

Continue developing this project in the [Lovable editor](https://lovable.dev/projects/f57def16-e765-4bcf-b429-4facc7f7834b).

- **Ship faster**: describe what you want to build and Lovable handles the code.
- **Stay in sync**: every change made in Lovable is committed straight to this repository.
- **Full ownership**: this code is yours. Push to `main` on GitHub and your changes sync back into Lovable, ready for your next prompt.

## Development

Prefer working locally? You need Node.js and npm — [install with nvm](https://github.com/nvm-sh/nvm#installing-and-updating).

```sh
git clone <this-repository-url>
cd <repository-name>
npm i
npm run dev
```
