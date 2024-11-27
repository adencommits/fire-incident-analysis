# Fire Incident Analysis with Data Structures

## Overview
This project analyzes fire incident data from the Greater Toronto Area (GTA) using two common data structures: a Linked List and a Binary Search Tree (BST). The goal is to evaluate and compare the performance of these structures when inserting and constructing trees from fire incident data.

The project loads data from a CSV file (`fires.csv`), creates instances of fire incidents, and builds both a Linked List and a Binary Search Tree. It then measures the insertion and construction times for each data structure as the number of fire incidents increases. The results are visualized in a set of plots to compare the performance of each data structure.

## Key Features
- **Fire Incident Class**: Stores information about each fire, such as the loss, responding personnel, cause, time, and geographical coordinates.
- **Linked List**: Implements a sorted linked list to store fire incidents based on the number of responding personnel.
- **Binary Search Tree (BST)**: Implements a BST to store fire incidents in a similar manner to the linked list, allowing comparison of performance for insertion and construction.
- **Performance Comparison**: Measures and compares the insertion times and construction times for both data structures.

## Requirements
- Python 3.x
- Matplotlib (for data visualization)
- CSV module (for reading the fire data)
  
## Installation
To get started with this project, follow the instructions below:

1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd <repository-directory>
   ```

2. Install the required dependencies:
   ```bash
   pip install matplotlib
   ```

3. Ensure you have the `fires.csv` file, which contains the fire incident data. You can use the example provided in the repository.

## Files Overview
- **fire_analysis.py**: This is the main script that performs the analysis. It includes the classes `Fire`, `LinkedListNode`, and `BSTTree`, as well as the functions to read data, build the data structures, and perform the performance analysis.
- **fires.csv**: A CSV file containing data on fire incidents. The columns include the estimated dollar loss, the number of responding personnel, the cause of the fire, the time of arrival, and the geographical coordinates.
- **output_plots**: After running the script, performance comparison plots are generated to show the insertion and construction time comparisons between the Linked List and BST.

## How to Run
1. Place the `fires.csv` file in the same directory as `fire_analysis.py`.

2. Run the Python script:
   ```bash
   python fire_analysis.py
   ```

3. The script will generate two plots:
   - **Insertion Time Plot**: Compares the time taken to insert fire incidents into the Linked List and BST.
   - **Construction Time Plot**: Compares the time taken to build the Linked List and BST from the data.

## Example CSV Format (`fires.csv`):
```csv
Estimated_Dollar_Loss,Number_of_responding_personnel,Possible_Cause,TFS_Arrival_Time,Latitude,Longitude
20000,47,52 - Electrical Failure,2020-01-01T00:46:05,43.71523573,-79.23910745
500,22,"98 - Unintentional, cause undetermined",2020-01-01T00:55:17,43.68760327,-79.35415411
...
```

## License
This project is licensed under the MIT License - see the LICENSE file for details.
```
