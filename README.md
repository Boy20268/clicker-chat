# Clicker Chat 🐶

A simple **two-person peer-to-peer chatroom** with a realistic dog-training clicker button.

## Features
- Private 1:1 chat (no accounts, no message storage on any server)
- Big tactile **CLICK** button that plays a classic clicker-training sound
- When connected, both people hear the click when either presses the button
- Works on mobile and desktop
- Uses PeerJS free cloud signaling + WebRTC data channels

## How to use

### Option 1 – GitHub Pages (recommended)
1. Go to the repository **Settings → Pages**
2. Under "Build and deployment" set Source to **Deploy from a branch**
3. Branch: `main` / folder: `/ (root)`
4. Save → wait ~1 minute
5. Your live site will be at:  
   **https://boy20268.github.io/clicker-chat/**

### Option 2 – Open locally
Just open `index.html` in any modern browser (Chrome, Firefox, Safari, Edge).

### How two people chat
1. Both open the page.
2. Copy your own Peer ID (the long random string).
3. One person pastes the other's ID and hits **Connect**.
4. Chat and click away!

The connection is direct peer-to-peer. Messages never touch a central server after the initial handshake.

## Technical notes
- PeerJS 1.5.5 + free 0.peerjs.com signaling
- Clicker sound is synthesized with Web Audio API (no external audio file)
- Fully offline-capable after first load (except signaling)
