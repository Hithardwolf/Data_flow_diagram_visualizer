# Data Flow Diagram (DFD) Visualizer

## 📖 Overview
A web-based DFD visualizer that parses structured JSON input and renders Data Flow Diagrams following standard DFD rules. Built with React and Vite.

## 🚀 Features
- JSON parser for DFD components
- Visual rendering using HTML5 Canvas
- Standard DFD shapes (processes, external entities, data stores, data flows)
- Trust boundary visualization based on deployment
- Interactive legend drawn on canvas
- Add processes directly through the UI
- Download diagrams as PNG

## 🧩 DFD Rules Implemented
- Process → Circle
- External Entity → Rectangle
- Data Store → Open rectangle
- Data Flow → Directed arrow
- Trust Boundary → Dashed red line

## 🛠 Tech Stack
- React 18 (with Hooks)
- Vite (build tool)
- HTML5 Canvas (rendering)
- Tailwind CSS (styling)
- Lucide React (icons)

## ▶️ How to Run
```bash
npm install
npm run dev
```

## 🏗 How to Build
```bash
npm run build
npm run preview
```

## 📝 Usage
1. Paste your DFD JSON in the input field
2. Click "Parse & Render" to visualize the diagram
3. Use "Add Process" to add new processes interactively
4. Click "Download PNG" to save the diagram

## 📄 JSON Format
```json
{
  "DFD features": {
    "external_entities": ["Users", "Store Admins"],
    "processes": ["Manage Purchases", "Manage Inventory"],
    "data_stores": ["Purchase Database", "Inventory Database"],
    "data_flows": ["1. Users → Manage Purchases → Purchase Database"],
    "deployment": "Hybrid Cloud Environment",
    "piidata": ["Customer Information"]
  }
}
```
