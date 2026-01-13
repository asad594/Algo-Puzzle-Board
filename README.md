# 🧩 AlgoPuzzleBoard MVC

**A stunning ASP.NET Core MVC application featuring interactive algorithm visualizations with a premium glassmorphism design.**

![.NET Version](https://img.shields.io/badge/.NET-9.0-512BD4?style=for-the-badge&logo=dotnet)
![C#](https://img.shields.io/badge/C%23-Backend-239120?style=for-the-badge&logo=csharp)
![License](https://img.shields.io/badge/License-MIT-yellow?style=for-the-badge)

---

## 🌟 Features

### ✅ Fully Implemented Algorithms

- **N-Queens Problem** - Backtracking algorithm with step-by-step visualization
- **Knight's Tour** - Warnsdorff's heuristic for efficient pathfinding
- **Graph Coloring** - Greedy coloring algorithm with interactive graph generation
- **Dijkstra's Algorithm** - Shortest path visualization with dynamic graph
- **Traveling Salesman Problem (TSP)** - Nearest neighbor + 2-opt optimization
- **Huffman Coding** - Tree construction and character encoding visualization

### 🎯 Key Functionalities

- **100% C# Backend** - All algorithm logic implemented in ASP.NET Core services
- **Real-time Visualization** - Interactive step-by-step algorithm execution
- **Score & Timer System** - Track performance and completion time
- **Hint System** - Get intelligent hints when stuck
- **Manual & Auto Modes** - Choose between guided solving or watching the algorithm
- **Responsive Design** - Works seamlessly on desktop, tablet, and mobile devices
- **Premium UI/UX** - Modern glassmorphism design with smooth animations

---

## 🚀 Running the Application

### Prerequisites

- [.NET 9.0 SDK](https://dotnet.microsoft.com/download/dotnet/9.0)
- Visual Studio Code (recommended) or Visual Studio 2022

### Using Terminal

1. **Open Terminal** in VS Code (`Ctrl + \``)

2. **Navigate to project directory:**
   ```bash
   cd "c:\Users\RB Tech\Desktop\MVC\AlgoPuzzleBoard.MVC"
   ```

3. **Run the application:**
   ```bash
   dotnet run
   ```

4. **Open your browser** and navigate to:
   ```
   http://localhost:5024
   ```

5. **Stop the application:** Press `Ctrl + C` in the terminal

### Using VS Code Debugger

1. Press `F5` or click **Run > Start Debugging**
2. Select **.NET Core** when prompted
3. The application will start and browser will open automatically

---

## 📁 Project Structure

```
AlgoPuzzleBoard.MVC/
├── Controllers/          # C# API Controllers for each algorithm
│   ├── NQueensController.cs
│   ├── KnightsTourController.cs
│   ├── GraphColoringController.cs
│   ├── DijkstraController.cs
│   ├── TSPController.cs
│   └── HuffmanController.cs
├── Services/            # C# Algorithm Implementations (ALL LOGIC IN C#)
│   ├── NQueensService.cs
│   ├── KnightsTourService.cs
│   ├── GraphColoringService.cs
│   ├── DijkstraService.cs
│   ├── TSPService.cs
│   └── HuffmanService.cs
├── Models/              # Data models and ViewModels
├── Views/               # Razor views (HTML templates)
│   ├── Home/
│   ├── NQueens/
│   ├── KnightsTour/
│   ├── GraphColoring/
│   ├── Dijkstra/
│   ├── TSP/
│   └── Huffman/
├── wwwroot/
│   ├── css/            # Stylesheets (glassmorphism design)
│   └── js/             # JavaScript (UI interactions only)
└── Program.cs          # Application entry point
```

---

## 🔌 API Endpoints

All algorithms run in **C#** and return **JSON** responses:

| Method | Endpoint | Description |
|--------|----------|-------------|
| `POST` | `/NQueens/Solve` | Returns backtracking solution steps |
| `POST` | `/KnightsTour/SolveTour` | Returns complete knight's tour path |
| `POST` | `/GraphColoring/GenerateGraph` | Generates random graph with nodes/edges |
| `POST` | `/GraphColoring/SolveColoring` | Returns colored graph solution |
| `POST` | `/Dijkstra/GenerateGraph` | Generates weighted graph for pathfinding |
| `POST` | `/Dijkstra/FindPath` | Returns shortest path between nodes |
| `POST` | `/TSP/SolveTSP` | Returns optimized TSP tour |
| `POST` | `/Huffman/BuildTree` | Returns Huffman tree and character codes |

---

## 🛠️ Technology Stack

| Layer | Technology |
|-------|-----------|
| **Backend Framework** | ASP.NET Core MVC (.NET 9.0) |
| **Programming Language** | C# (100% backend logic) |
| **Frontend** | HTML5, CSS3, JavaScript (ES6+) |
| **Design System** | Glassmorphism with gradient animations |
| **Architecture** | MVC Pattern with Service Layer |

---

## 🎨 Design Philosophy

- **Premium Aesthetics** - Glassmorphism effects with vibrant gradients
- **Smooth Animations** - Micro-interactions for enhanced UX
- **Responsive Layout** - Mobile-first design approach
- **Accessibility** - WCAG compliant color contrasts and keyboard navigation

---

## 💻 Development Commands

### Build the project
```bash
dotnet build
```

### Clean build artifacts
```bash
dotnet clean
```

### Run with auto-reload (watch mode)
```bash
dotnet watch run
```

### Restore dependencies
```bash
dotnet restore
```

---

## 📚 Algorithm Details

### N-Queens Problem
Solves the classic N-Queens puzzle using **backtracking**. Place N queens on an N×N chessboard so no two queens threaten each other.

### Knight's Tour
Implements **Warnsdorff's Rule** to find a path where a knight visits every square on a chessboard exactly once.

### Graph Coloring
Uses a **greedy coloring algorithm** to assign colors to graph nodes such that no adjacent nodes share the same color.

### Dijkstra's Algorithm
Finds the **shortest path** between nodes in a weighted graph using Dijkstra's classic algorithm.

### Traveling Salesman Problem (TSP)
Optimizes the shortest route visiting all cities using **nearest neighbor** initialization and **2-opt** local search.

### Huffman Coding
Builds a **Huffman tree** for optimal character encoding based on frequency analysis.

---

## 🎯 Key Highlights

✨ **All algorithm logic is implemented in C# backend services**  
✨ **JavaScript is only used for UI interactions and AJAX calls**  
✨ **RESTful API design for algorithm endpoints**  
✨ **Real-time visualization with step-by-step control**  
✨ **Modern, premium UI with glassmorphism design**  
✨ **Fully responsive across all devices**

---

## 📄 License

This project is licensed under the MIT License.

---

## 👨‍💻 Author

**RB Tech**

---

## 🙏 Acknowledgments

Built with ❤️ using ASP.NET Core MVC and modern web technologies.

---

**Note:** All algorithm implementations are in C# backend services. JavaScript files in `wwwroot/js/` are exclusively for UI interactions, DOM manipulation, and calling the C# APIs via AJAX.
