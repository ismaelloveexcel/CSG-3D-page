# CSG-based ML-supported 3D translation of sketches into game assets for game designers

A web application that translates 2D sketches into 3D models in real-time. This project allows users to draw 2D sketches of walls and automatically converts them into a 3D representation.

**Read our paper here**: [CSG-based ML-supported 3D translation of sketches into game assets for game designers](https://link.springer.com/article/10.1007/s00371-024-03758-9)

## Features

- **Interactive Sketch Canvas**
  - Draw using multiple tools (Rectangle, Circle, Free-hand)
  - Eraser tool for corrections
  - Adjustable canvas size (width and height)
  - Clear canvas functionality

- **Multi-Wall Support**
  - Draw on four different walls (Front, Right, Back, Left)
  - Easy navigation between walls
  - Progress bar for wall depth adjustment

- **Real-time 3D Rendering**
  - Instant conversion of 2D sketches to 3D models
  - Interactive 3D viewer with orbit controls
  - Export functionality to OBJ format

## Technologies Used

- Frontend:
  - Three.js for 3D rendering
  - HTML5 Canvas for 2D sketching
  - CSS3 for styling and animations
  - Vanilla JavaScript for interactivity

## Deploy on Replit

You can deploy this project page directly on Replit:

1. Click the button below to import this repository into Replit:

   [![Run on Replit](https://replit.com/badge/github/ismaelloveexcel/CSG-3D-page)](https://replit.com/github/ismaelloveexcel/CSG-3D-page)

2. Alternatively, you can manually import:
   - Go to [Replit](https://replit.com)
   - Click "Create Repl" → "Import from GitHub"
   - Paste the repository URL: `https://github.com/ismaelloveexcel/CSG-3D-page`
   - Click "Import from GitHub"

3. Once imported, click the "Run" button to start the server
4. The project page will be available at the URL provided by Replit

## Setup and Installation

1. Clone the repository:
```bash
git clone https://github.com/Spectraorder/sketch-3d-translation.git
cd sketch-3d-translation
```

2. Set up the environment:

It is recommended to use Conda to create a clean environment for managing dependencies:
```bash
conda create --name sketch3d python=3.10
conda activate sketch3d
```

3. Install dependencies:

Update pip and install the required libraries from requirements.txt:
```bash
python -m pip install --upgrade pip
pip install -r requirements.txt
```

- For systems with CUDA support:
```bash
pip install torch==2.2.1 torchvision==0.17.1 torchaudio==2.2.1 --index-url https://download.pytorch.org/whl/cu118
```
Replace cu118 with your CUDA version if different.

- For systems without CUDA (CPU-only):
```bash
pip install torch==2.2.1 torchvision==0.17.1 torchaudio==2.2.1
```

3. Run the application:
```bash
python main.py
```
The application will start using Flask. By default, it will run on `http://127.0.0.1:5000/`.
Open this URL in a modern web browser to use the application.

## Usage

1. Use the sketch canvas to draw your 2D design
2. Select different drawing tools from the toolbar:
   - Rectangle tool for straight edges
   - Circle tool for curved surfaces
   - Eraser tool for corrections
3. Navigate between different walls using the arrow buttons
4. Adjust wall depth using the progress bar
5. View the 3D model in real-time in the right panel
6. Export the final 3D model as needed

## Citation

If you find this repo useful for your research, please consider citing our paper

```
@article{Chen2025,
  author    = {Y. Chen and Y. Liu and G. Kayar-Ceylan},
  title     = {CSG-based ML-supported 3D translation of sketches into game assets for game designers},
  journal   = {The Visual Computer},
  year      = {2025},
  doi       = {10.1007/s00371-024-03758-9},
  note      = {Accepted: 08 December 2024, Published: 05 January 2025}
}

```

This version includes instructions for installing dependencies and running the application with Flask. Let me know if you need further adjustments!