# Environmental Pollution Tracker System

A comprehensive C++ application designed to monitor, analyze, and manage environmental pollution data across multiple geographical locations. This system integrates various data structures to provide efficient data management, hierarchical organization, and analytical capabilities.

## 🚀 Features

### 1. Pollution Management
- Track pollution levels for Air, Water, Soil, and Noise.
- **Data Structures**: Linked List for dynamic record storage.
- **Key Capabilities**:
  - Add, search, and delete records.
  - Automatic severity classification (Low/Medium/High).
  - Safety alert generation.
  - Trend predictions.

### 2. Complaint Management
- Manage citizen complaints regarding environmental issues.
- **Data Structures**: Linked List.
- **Key Capabilities**:
  - Submit and track complaints.
  - Auto-priority calculation.
  - Filter by status (Pending/Resolved).
  - Resolution statistics.

### 3. Sensor Management
- Simulates real-time data collection from sensors.
- **Data Structures**: Queue (for processing), Static Arrays, Sensor Manager.
- **Key Capabilities**:
  - Simulated sensor readings.
  - Fault detection and handling.
  - Emergency shutdown by area.
  - Queue-based processing for fair data handling.

### 4. Area Tree (Geographical Hierarchy)
- Hierarchical organization of locations (Country -> City -> Area -> Sensor).
- **Data Structures**: N-ary Tree.
- **Key Capabilities**:
  - Visual display of location hierarchy.
  - Easy navigation and management of areas.
  - Auto-loads from `tree_data.txt`.

### 5. Pollution Graph (Connectivity & Spread)
- Models connectivity between different areas to analyze pollution spread.
- **Data Structures**: Adjacency Matrix (Graph).
- **Key Capabilities**:
  - Analyze how pollution spreads between connected areas.
  - Identify highly polluted clusters.
  - Syncs automatically with the Area Tree.

### 6. Reports & Analytics
- Generate comprehensive reports on pollution trends, complaint resolutions, and safety alerts.

### 7. Undo System
- Robust undo functionality for critical operations (Add/Delete).
- **Data Structures**: Stack.

## 🛠️ Technical Details

- **Language**: C++ (Standard 98/03/11 compatible)
- **Persistence**: File-based storage (CSV and Text files).
  - `pollution_data.txt`
  - `complaint_data.txt`
  - `sensor_data.txt`
  - `tree_data.txt`
- **Interface**: Console-based Menu System.

## 📋 Prerequisites

- A C++ Compiler (GCC, MinGW, Clang, or Visual Studio Build Tools).
- Windows/Linux/macOS terminal.

## ▶️ How to Run

1.  **Compile the code**:
    Open your terminal/command prompt and navigate to the project directory. Run:
    ```bash
    g++ ALL_IN_ONE.cpp -o pollution_tracker
    ```

2.  **Run the application**:
    ```bash
    ./pollution_tracker
    ```
    *(On Windows, you can just type `pollution_tracker` or double-click the `.exe` file if created).*

## 📂 File Structure

- `ALL_IN_ONE.cpp`: Main source code file containing all classes and logic.
- `PROJECT_REPORT.md`: Detailed project documentation.
- `*.txt`: Data files for persistence.

## 🔮 Future Enhancements
- Database integration (SQL).
- Web/Mobile app interface.
- Real-time IoT sensor integration.
- Graphical visualizations.
