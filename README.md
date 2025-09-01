# Unilog Flowchart

This repository contains the flowchart and HTML viewer for the Unilog (InternTrack) eLogbook system.

What’s included
- `flowchart TD.txt` — mermaid flowchart source (text)
- `index.html` — simple HTML page that renders the flowchart using Mermaid via CDN

Recent fix
- The flowchart now explicitly returns unauthenticated users to the login page when authentication fails.

How to view
1. Open `index.html` in a browser (double-click). Mermaid is loaded from CDN and the diagram will render on page load.
2. Or serve the folder with a simple HTTP server (recommended to avoid some browser file restrictions):

   # Using Python 3
   python -m http.server 8000

   Then open http://localhost:8000

Notes
- The mermaid diagram uses `securityLevel: 'loose'` to allow HTML line breaks inside nodes.
- Edit the flowchart by updating `flowchart TD.txt` and reloading `index.html`.

License
- No license specified. Add a LICENSE file if you want to make this project open source.

Contact
- For questions, modify the repo or open an issue in the upstream GitHub repository.
