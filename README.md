# cello.

**A Gesture-Controlled Virtual String-Instrument Studio**

Cello is a browser-based application that translates hand gestures into musical events using computer vision and real-time audio processing. It aims to provide an interactive virtual instrument experience through webcam-based hand tracking and gesture recognition.

The planned instruments include acoustic guitar, electric guitar, bass guitar, and ukulele.

## Overview

Cello combines hand tracking, gesture recognition, musical-event mapping, and browser-based audio generation to create a responsive musical interface.

### Planned Features

- **Hand Tracking:** Detect and visualize hand landmarks using MediaPipe.
- **Gesture Recognition:** Identify deliberate hand movements, including directional strumming gestures.
- **Real-Time Audio:** Translate recognized gestures into sound using the Web Audio API and Tone.js.
- **Interactive Interface:** Provide tracking feedback, audio controls, and instrument selection.
- **Calibration and Diagnostics:** Support gesture adjustment and performance evaluation.

Features will be marked as implemented and tested as development progresses.

## Technology Stack

| Category | Technologies |
|---|---|
| Frontend | React, Vite, TypeScript |
| Styling and Animation | Tailwind CSS, Motion for React |
| Computer Vision | MediaPipe Hand Landmarker |
| Audio Processing | Web Audio API, Tone.js |
| Testing | Vitest, React Testing Library, Playwright |
| Code Quality | ESLint, Prettier |
| Version Control | Git, GitHub |

## Development Roadmap

The initial milestone focuses on establishing a functional webcam-to-audio pipeline:

1. Implement webcam access and permission handling.
2. Integrate hand-landmark detection and visualization.
3. Develop a basic directional gesture recognizer.
4. Map recognized gestures to musical events.
5. Trigger audio with visual feedback.
6. Validate reliability, responsiveness, and resource cleanup.

Further development may include additional instruments, gesture calibration, chord interaction, recording, and performance diagnostics.

## Getting Started

### Prerequisites

- Node.js and npm
- Git
- A modern browser with webcam and audio support

### Installation

```bash
git clone <repository-url>
cd <repository-folder>
npm install
npm run dev
```

Replace the placeholders with the actual repository URL and directory. Run the commands from the directory containing the relevant `package.json`.

Open the local URL provided by Vite. Grant camera permission when prompted. Browser audio playback may require an initial user interaction.

## Testing and Quality Assurance

The project will use automated tests for gesture-recognition logic, interface behavior, and browser workflows. Manual testing will validate webcam tracking, audio output, performance, and resource management.

Where configured, run:

```bash
npm run lint
npm run build
```

A successful build does not independently verify webcam tracking or audio functionality.

## Privacy

The intended architecture processes webcam input locally in the browser. Camera access should require user permission, and media resources should be released when no longer needed. Privacy claims will be confirmed against the implemented data flow.

## Project Status

Cello is under development. The initial priority is to validate the core interaction pipeline before expanding instrument support or introducing advanced features.

## License

A license has not yet been specified. Licensing details will be added before distribution. Third-party audio assets must comply with their respective licenses.
