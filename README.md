
# Parking Spot Finder

This program helps identify and track free parking spots in a parking lot using an image of the lot. It allows users to select parking spots on an image and automatically checks their availability.

## Features
- **Interactive Spot Selection**: Users can select parking spots on the image by drawing boxes.
- **Box Management**: 
  - Left-click to create/select boxes for parking spots.
  - Right-click to remove wrongly selected boxes.
- **Spot Tracking**: The program tracks the selected spots and checks if they are free or occupied.
- **Count Display**: The count of free spots is displayed on the image.

## Getting Started

### Prerequisites
- Python 3.x
- OpenCV Library
- Pickle Library (comes pre-installed with Python)

### Installation
1. Clone the repository or download the project files.
2. Ensure `carParking.png` (or your parking lot image) is in the project directory.
3. Install required dependencies:
   ```bash
   pip install opencv-python
   ```

### How to Use
1. **Run the Script**:
   - Start by running the `parkfinding.py` file:
     ```bash
     python parkfinding.py
     ```
   - The program will display the parking lot image (`carParking.png`).

2. **Select Parking Spots**:
   - Use your mouse to draw boxes around the parking spots on the displayed image.
   - Each box represents a parking spot.

3. **Manage Spots**:
   - **Add Spots**: Draw boxes by clicking and dragging.
   - **Remove Spots**: Right-click on an existing box to remove it.

4. **Save Selected Spots**:
   - Once you have selected the desired spots, the program will create a file (using the `pickle` library) to store the box positions.

5. **Check Availability**:
   - After initializing the spots, the program will monitor the parking spaces and determine if they are free or occupied.
   - The count of free spots will be displayed at the top of the image.

6. **Exit**:
   - Press the `q` key to quit the program.

## File Structure
- `parkfinding.py`: Main script for running the program.
- `carParking.png`: Image of the parking lot (replace with your own image if needed).
- `boxes.pkl`: Automatically generated file that stores the parking spot positions.

## Notes
- Ensure that `carParking.png` is a clear and well-lit image for better accuracy.
- You can replace `carParking.png` with any other parking lot image, but you may need to reselect the spots.

