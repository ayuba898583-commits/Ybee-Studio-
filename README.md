# Y BEE STUDIO — starter app

This is the first runnable prototype of Y BEE STUDIO.

## Included in version 1
- Dark studio interface
- Microphone permission and high-quality vocal recording
- Import an instrumental audio file from the iPhone Files picker
- Play the imported beat
- Play back a recorded vocal take
- Share/export the vocal take using the iOS share sheet

## Important scope note
This first build does **not** yet mix the beat and vocal together, record while the beat is playing, apply AutoTune/effects, or export a mastered stereo song. Those need the next audio-engine development stage. The app currently previews the beat and vocal separately so the recording workflow can be tested safely.

## What you need
- A Windows PC or Mac with Node.js LTS installed
- The Y_BEE_STUDIO project folder unzipped on that computer
- An iPhone with the App Store version of Expo Go installed (this starter uses Expo SDK 54 for compatibility), and an Expo account

## Install and run
Open Terminal (Mac) or PowerShell (Windows) inside this folder and run:

```bash
npm install
npx expo install expo-audio expo-document-picker expo-sharing
npx expo install --fix
npx expo start
```

If prompted to install compatible Expo packages, accept the suggested versions.

1. Connect the iPhone and computer to the same Wi-Fi network.
2. Open Expo Go on the iPhone and sign in to the same Expo account used by the CLI if prompted.
3. Scan the QR code shown in the terminal using the iPhone Camera app.
4. Open the project in Expo Go.
5. Allow microphone access when iOS asks.

If the project does not open in Expo Go because of SDK compatibility, use the development-build path in the Expo documentation. A production installable iPhone app requires signing/build configuration.

## Notes
- Recording files are initially held in the app's temporary/cache storage. Export/share each take you want to keep.
- Headphones are recommended when monitoring or recording to avoid speaker feedback.
- For low-latency monitoring, simultaneous beat playback and vocal recording, effects, and a combined mixdown, we will add a dedicated audio engine in a later stage.

