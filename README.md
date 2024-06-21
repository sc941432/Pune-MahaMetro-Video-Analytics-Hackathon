Got it. I'll update the README with the correct paths for the images. Here is the revised README:

---

# VA-Hackathon Pune-MahaMetro Video Analytics Solutions

Welcome to the VA-Hackathon Pune-MahaMetro project! This repository contains solutions developed for two critical safety issues observed in Pune MahaMetro stations:

1. Platform Edge Fall Detection
2. Escalator Fall Detection

## Project Structure

The project is organized into two main folders:

- `Platform-Edge Fall Detection`
  - `Platform-Edge.ipynb`
  - `best_segment_old.pt`
  - `yolov8s.pt`
  - `Screenshot 2024-05-03 154200.png`
- `Esclator Fall Detection`
  - `fall.ipynb`
  - `best_our.pt`
  - `Screenshot 2024-05-03 154250.png`

## Problem Statements

### Platform Edge Fall Detection

**Problem:**
The fall of passengers on the track is a major safety concern, often occurring when passengers cross the platform edge while looking for the train. This can result in serious accidents or train overruns.

**Solution:**
Using video analytics on CCTV cameras installed on platforms, we have developed a model to detect passengers crossing the platform edge. The system triggers real-time alerts to avert accidents. This model uses segment detection for higher accuracy in identifying the platform edge and potential falls.

**Files:**
- `Platform-Edge.ipynb`: Jupyter notebook containing the implementation of the platform edge fall detection model.
- `best_segment_old.pt`: Trained model file for segment detection.
- `yolov8s.pt`: Pre-trained YOLOv8 model file used for initial object detection.

### Escalator Fall Detection

**Problem:**
The fall of passengers on escalators is another significant safety concern. Timely detection and alerts are crucial to prevent injuries and accidents.

**Solution:**
We developed a video analytics solution using a dedicated CCTV camera view of the escalator to identify fall cases. The system triggers real-time alerts to ensure passenger safety. This model uses rectangular bounding box detection for identifying falls on the escalator.

**Files:**
- `fall.ipynb`: Jupyter notebook containing the implementation of the escalator fall detection model.
- `best_our.pt`: Trained model file for detecting falls using bounding boxes.

## Installation and Usage

1. Clone the repository:

    ```bash
    git clone https://github.com/sc941432/Pune-MahaMetro-Video-Analytics-Hackathon.git
    cd Pune-MahaMetro-Video-Analytics-Hackathon
    ```

2. Set up the Python environment:

    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
    pip install -r requirements.txt
    ```

3. Run the Jupyter notebooks:

    ```bash
    jupyter notebook
    ```

4. Open `Platform-Edge.ipynb` or `fall.ipynb` and follow the instructions to run the models.

## Model Details

### Platform Edge Fall Detection

- **Approach**: Segment detection
- **Model Files**:
  - `best_segment_old.pt`
  - `yolov8s.pt`

### Escalator Fall Detection

- **Approach**: Bounding box detection
- **Model Files**:
  - `best_our.pt`

## Images

### Platform Edge Fall Detection
![Platform Edge Fall Detection](Platform-Edge%20Fall%20Detection/Screenshot%202024-05-03%20154200.png)

### Escalator Fall Detection
![Escalator Fall Detection](Esclator%20Fall%20Detection/Screenshot%202024-05-03%20154250.png)

## License

This project is licensed under the MIT License. See the LICENSE file for more details.

## Acknowledgements

Special thanks to the organizers of the VA-Hackathon and Pune MahaMetro for providing the opportunity to work on these safety-critical solutions.

---

Feel free to reach out for any questions or collaboration opportunities.

---

Make sure the paths to the images in the `README` match the exact paths and filenames in your repository.
