# Fire Incident Data Analysis: Linked List vs Binary Search Tree

This project analyzes fire incident data from the Greater Toronto Area (GTA) by comparing the performance of a Linked List and a Binary Search Tree (BST) for storing and processing fire data. It measures and visualizes insertion and construction times for each data structure.

## Project Structure

### 1. `fire_incident_analysis.py`

This script processes fire data, builds a linked list and binary search tree, and measures the performance of both data structures. Key components include:

- **Fire class**: Represents a fire incident, storing relevant data such as loss amount, number of responding personnel, cause, time, and location.
- **LinkedListNode class**: Implements a linked list data structure to store fire incidents in sorted order based on the number of responding personnel.
- **BSTTree class**: Implements a binary search tree to store fire incidents and perform insertions efficiently.
- **Main execution**: The script reads fire data from a CSV file, constructs both data structures, measures performance, and visualizes the results using Matplotlib.

### 2. `fires.csv`

This CSV file contains the fire incident data. The columns in the file are:

- `Estimated_Dollar_Loss`: Dollar value of the fire damage.
- `Number_of_responding_personnel`: Number of personnel who responded to the fire.
- `Possible_Cause`: The potential cause of the fire.
- `TFS_Arrival_Time`: The timestamp when Toronto Fire Services arrived at the scene.
- `Latitude`: Latitude of the incident location.
- `Longitude`: Longitude of the incident location.

```csv
Estimated_Dollar_Loss,Number_of_responding_personnel,Possible_Cause,TFS_Arrival_Time,Latitude,Longitude
20000,47,52 - Electrical Failure,2020-01-01T00:46:05,43.71523573,-79.23910745
500,22,"98 - Unintentional, cause undetermined",2020-01-01T00:55:17,43.68760327,-79.35415411
1000,30,"Fire - Unknown Cause",2020-01-01T01:05:10,43.75849216,-79.31223325
```

### 3. Performance Measurements

The script measures and compares the following for both the Linked List and the Binary Search Tree:

- **Insertion Time**: The time it takes to insert fire incidents into each data structure.
- **Construction Time**: The time it takes to build the entire linked list or binary search tree from a set of fire incidents.

The results are plotted using Matplotlib to visually compare the performance of the two data structures as the number of fire incidents increases.

### 4. Example Usage

1. Ensure you have the required libraries installed:

    ```bash
    pip install matplotlib
    ```

2. Run the script:

    ```bash
    python fire_incident_analysis.py
    ```

3. The script will generate two plots:
   - **Insertion Time**: A comparison of how long it takes to insert fire incidents into the Linked List and the Binary Search Tree.
   - **Construction Time**: A comparison of the time taken to construct the entire data structure.

### 5. License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
