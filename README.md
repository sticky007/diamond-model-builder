# Diamond Model CTI Tool

A professional drag-and-drop Diamond Model diagramming tool for CTI analysts.

## Features
- Drag and drop Adversary, Capability, Infrastructure, Victim, Event nodes
- IOC / Data Table nodes with editable columns and rows
- Connect Mode — click two nodes to draw edges
- Arrow styles: solid, dashed, dotted, bidirectional, line only
- Line color picker + custom color
- Line thickness control
- Title and body text size controls
- Drag to reposition nodes
- Resize nodes with corner handle
- Double-click any node to open full edit modal
- Add/remove content lines in modal
- Delete nodes/edges with Delete key or button
- Export SVG, PNG, JSON
- Import JSON to restore diagrams
- Pre-loaded Tycoon 2FA example

## Run with Docker

```bash
docker-compose up --build
```

Then open: http://localhost:5000

## Run without Docker

```bash
pip install flask
python app.py
```

Then open: http://localhost:5000

## Usage

1. **Add nodes** — drag chips from the left panel onto the canvas
2. **Connect nodes** — click "Connect Mode", then click two nodes
3. **Edit content** — double-click any node, or use the Properties panel on the left
4. **Style edges** — click an edge to select it, then change arrow style/color/width
5. **Resize** — drag the small square at the bottom-right corner of any node
6. **Delete** — select anything and press Delete, or use the Delete button in Properties
7. **Export** — SVG for vector, PNG for presentation, JSON to save and reload

## Diamond Model Vertices

| Vertex | Color | Description |
|---|---|---|
| Adversary | Red | Threat actor, group, or individual |
| Capability | Amber | Tools, malware, TTPs used |
| Infrastructure | Purple | Domains, IPs, hosting used |
| Victim | Teal | Target organization or individual |
| Intrusion Event | Blue | The event connecting all four vertices |
| IOC Table | Green | Structured indicator data |

## Creator & License

**Author**: Sticky Afrojack  
**Contact**: sticky.afrojack@proton.me  
**Version**: Diamond Model Builder V1  
**License**: MIT

This tool is built for CTI analysts to create threat intelligence diagrams using the Diamond Model framework.

---

© 2026 Sticky Afrojack. Licensed under MIT.
