# Inventory-management-project-using-OOP
This is a project that implements an inventory management system using Object oriented programming. This supports setting and removing the items using First In First Out (FIFO) logic and also using specific IDs of the items. 

# Shelf Space Management System

This project provides the functionality to manage shelf spaces for a robot system. It includes an interface for the robot to manage the storage, removal, and retrieval of parts in a warehouse or inventory system.

## Required Functionality

The system implements the following functionality:

- **Get Next Free Shelf Space**: The robot can get the next available free shelf space.
- **Store a Part in the Next Free Shelf Space**: The robot can store a part in the next available shelf space.
- **Get Next Occupied Shelf Space**: The robot can retrieve the next occupied shelf space.
- **Remove/Unload Part**: The robot can remove/unload a part from the next occupied shelf space.
- **Get Shelf Space by Part ID**: The robot can get the shelf space corresponding to a specific part ID.
- **Put/Remove Part to/from Explicit Shelf Space**: The robot can place or remove parts from a specified shelf space.

## Installation and Setup

1. **Software Requirements**:
   - TwinCAT 2 or 3
   - Use either **Structured Text (ST)** or **Sequential Function Chart (SFC)** programming languages.

2. **Steps to Run the Project**:
   - Open the project in TwinCAT3.
   - Load and run the program on a robot or simulation system that is compatible with the `fbRobot` and `fbShelfManager` function blocks.

3. **No Persistence**:
   - This project does not require persistence, meaning no data is saved when the system stops.

## Project Structure

- **Main Program**: `MAIN` program contains the overall logic for managing the shelf spaces.
- **Function Blocks**:
   - `FB_Robot`: Manages robot-related operations, such as loading/unloading parts.
   - `FB_ShelfManager`: Manages the shelf spaces and handles the logic for placing/removing parts in/from the shelves.
   - `FB_QueueLogic`: Handles the queue logic used for getting and managing free/occupied shelf spaces.
