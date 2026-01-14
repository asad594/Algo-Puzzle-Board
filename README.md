# AlgoPuzzleBoard MVC
ASP.NET Core MVC application with C# backend for algorithm visualizations.

## Running the Application in Visual Studio Code
### Using Terminal
Open Terminal in VS Code (`Ctrl + ` `)

Navigate to project directory (if not already there):

```bash
cd "c:\Users\RB Tech\Desktop\MVC\AlgoPuzzleBoard.MVC"
```
Run the application:

```bash
dotnet run
```
Open your browser and navigate to:

[http://localhost:5024](http://localhost:5024)

Stop the application: Press `Ctrl + C` in the terminal

### Using VS Code Debugger
1. Press `F5` or click **Run > Start Debugging**
2. Select **.NET Core** when prompted
3. The application will start and browser will open automatically

## Project Structure
```text
AlgoPuzzleBoard.MVC/
├── Controllers/          # C# API Controllers
├── Services/            # C# Algorithm Implementations (ALL ALGORITHMS IN C#)
├── Models/              # Data models
├── Views/               # Razor views (HTML)
├── wwwroot/
│   ├── css/            # Stylesheets
│   └── js/             # JavaScript (UI only)
└── Program.cs          # App entry point
```

## Features
### Fully Implemented
✅ **N-Queens** - Backtracking algorithm visualization  
✅ **Knight's Tour** - Warnsdorff's heuristic  
✅ **Graph Coloring** - Greedy coloring (basic)  

### C# Backend Ready
🔧 **TSP** - Nearest neighbor + 2-opt optimization  
🔧 **Huffman Coding** - Tree construction and encoding  
🔧 **Pathfinding** - Dijkstra, BFS, DFS, Prim's, Kruskal's
🔧 **Sorting** - Quick, Merge, Heap, Radix, Bubble
🔧 **Search** - Linear, Binary, Interpolation
🔧 **Trees** - BST, Min Heap, Max Heap

## Technology Stack
*   **Backend**: ASP.NET Core MVC (.NET 9.0)
*   **Algorithms**: 100% C# (in `Services/`)
*   **Frontend**: HTML, CSS, JavaScript (UI interactions only)
*   **Design**: Glassmorphism with modern gradients

## API Endpoints
All algorithms run in C# and return JSON:

*   `POST /NQueens/Solve` - Returns backtracking solution steps
*   `POST /KnightsTour/SolveTour` - Returns tour path
*   `POST /GraphColoring/GenerateGraph` - Generates random graph
*   `POST /GraphColoring/SolveColoring` - Returns colored graph
*   `POST /TSP/SolveTSP` - Returns optimized tour
*   `POST /Huffman/BuildTree` - Returns Huffman tree and codes

## Development
### Build
```bash
dotnet build
```
### Clean
```bash
dotnet clean
```
### Watch (auto-reload on changes)
```bash
dotnet watch run
```

> **Note**: All algorithm logic is implemented in C# backend services. JavaScript is only used for UI interactions and calling the C# APIs via AJAX.
