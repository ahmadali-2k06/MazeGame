# 🧩 AlgoMaze - Pathfinding Visualizer

AlgoMaze is an interactive tool designed to help developers and students understand how pathfinding algorithms navigate complex environments. Built using the modern **.NET 8** stack, it provides a sleek, terminal-inspired interface with responsive animations and real-time audio feedback.

---

## 🚀 Features

* **Algorithm Visualization:** Real-time visualization of Breadth-First Search (BFS) and Depth-First Search (DFS).
* **Maze Generation:** Automatically generate complex layouts using:
* **Recursive Backtracker:** Creates a perfect, loop-free maze.
* **Recursive Division:** A grid-like approach to wall creation.
* **Spiral Pattern:** A satisfying geometric wall placement.


* **Interactive Editing:**
* **Drag & Drop:** Move the Start and Target nodes anywhere on the grid.
* **Draw Walls:** Click and drag to create custom obstacles.


* **Immersive Audio:** Integrated sound effects for wall creation, maze completion, and algorithm progress (with a Mute toggle).
* **Responsive UI:** Styled with **Tailwind CSS** for a dark-mode, high-tech aesthetic.

---

## 🛠️ Tech Stack

* **Frontend:** [Blazor WebAssembly](https://dotnet.microsoft.com/en-us/apps/aspnet/web-apps/blazor) (C#)
* **Styling:** [Tailwind CSS](https://tailwindcss.com/)
* **Icons & Fonts:** Google Material Symbols & Space Grotesk

---

## 📁 Folder Structure

```text
AlgoMaze/
├── .gitignore               # Configured to ignore bin/obj and local caches
├── MazeGame.sln             # Visual Studio Solution file
└── MazeGame/                # Primary Project Folder
    ├── Pages/
    │   └── Visualizer.razor # Core logic (BFS, DFS, Maze Gen, UI)
    ├── Layout/
    │   └── EmptyLayout.razor # Minimal layout for the visualizer
    ├── wwwroot/
    │   ├── assets/          # Audio files (.mp3/.ogg) and favicon
    │   ├── index.html       # Entry point with JS Audio Interop
    │   ├── favicon.png      # Custom Project Icon
    │   └── vercel.json      # Vercel-specific routing configuration
    ├── Program.cs           # Application startup
    └── MazeGame.csproj      # Project configuration and dependencies

```

---

## ⚙️ Local Setup

Follow these steps to get the project running on your local machine:

### Prerequisites

* [.NET 8.0 SDK](https://dotnet.microsoft.com/en-us/download/dotnet/8.0)
* Visual Studio 2022 (or VS Code with C# Dev Kit)

### Installation

1. **Clone the Repository:**
```bash
https://github.com/ahmadali-2k06/MazeGame
cd MazeGame/MazeGame

```


2. **Restore Dependencies:**
```bash
dotnet restore

```


3. **Run the Project:**
```bash
dotnet watch

```


*The app will automatically open in your browser at `https://localhost:5001` or `http://localhost:5000`.*

---

## 🖱️ How to Use

1. **Select an Algorithm:** Choose between BFS (Guaranteed shortest path) or DFS (Exploring deep branches) from the sidebar.
2. **Adjust Speed:** Use the range slider to slow down the visualization to see the logic step-by-step or speed it up for large grids.
3. **Generate a Maze:** Use the "Pattern" dropdown to select a generation method and click **Generate**.
4. **Custom Walls:** Use your mouse to draw walls directly on the grid to challenge the algorithm.
5. **Visualize:** Hit the **VISUALIZE** button and watch the algorithm find the path!
6. **Toggle Sound:** Use the volume icon in the top-left to enable or disable audio feedback.

---
