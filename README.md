<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Automatic Number Plate Recognition (ANPR)</title>
</head>
<body>
    <h1>Automatic Number Plate Recognition (ANPR) System 🚗📸</h1>
    <p>
        This repository contains the implementation of a robust <strong>Automatic Number Plate Recognition (ANPR)</strong> system designed to detect and recognize vehicle license plates in real-time or from video recordings. 
        The project leverages state-of-the-art machine learning models, efficient computer vision techniques, and robust OCR solutions to deliver accurate and scalable results.
    </p>

<h2>Key Features</h2>
    <ul>
        <li><strong>Vehicle and License Plate Detection</strong>: Utilizes <strong>YOLOv8</strong> for real-time detection of vehicles and license plates with high accuracy.</li>
        <li><strong>Optical Character Recognition (OCR)</strong>: Integrates <strong>PaddleOCR</strong> to extract text from detected license plates with character mapping and format validation for improved accuracy.</li>
        <li><strong>Vehicle Tracking</strong>: Implements the <strong>SORT algorithm</strong> to track vehicles across video frames, ensuring consistent identification of moving vehicles.</li>
        <li><strong>Data Management</strong>: Saves detection results (bounding boxes, license plate text, and confidence scores) in a structured CSV file with data interpolation for smooth transitions.</li>
        <li><strong>Visualization and Output</strong>: Annotates video frames with bounding boxes, license plate text, and cropped license plate images, producing a fully annotated video.</li>
    </ul>

  <h2>Project Structure</h2>
    <ul>
        <li><code>main.py</code>: The central script to run the ANPR system. Handles video input, detection, and result generation.</li>
        <li><code>util.py</code>: Utility functions for OCR, character mapping, CSV writing, and format validation.</li>
        <li><code>visualize.py</code>: Annotates video frames with detected vehicles and license plates, creating an output video.</li>
        <li><code>add_missing_data.py</code>: Handles interpolation of missing bounding box data for smoother tracking.</li>
        <li><code>requirements.txt</code>: Lists all dependencies required to run the system.</li>
    </ul>

 <h2>How to Use</h2>
    <ol>
        <li>Clone the repository:
            <pre><code>git clone https://github.com/your-username/anpr-system.git
cd anpr-system</code></pre>
        </li>
        <li>Install dependencies:
            <pre><code>pip install -r requirements.txt</code></pre>
        </li>
        <li>Run the main script:
            <pre><code>python main.py --video_path ./input_video.mp4 --output_path ./output_video.mp4</code></pre>
        </li>
        <li>Visualize results: The output video with annotations will be saved in the specified location.</li>
    </ol>

 <h2>Resources</h2>
    <ul>
        <li><strong>Final Result of the Project</strong>: <a href="https://drive.google.com/file/d/1jxp4Hu49lzS_gZ6qjB_0-HL4Y4pzu_Xm/view" target="_blank">View Here</a></li>
        <li><strong>Dataset Used (Annotated)</strong>: <a href="https://universe.roboflow.com/roboflow-universe-projects/license-plate-recognition-rxg4e/dataset/4" target="_blank">View on Roboflow</a></li>
    </ul>

 <h2>Applications</h2>
    <ul>
        <li>Traffic monitoring and enforcement</li>
        <li>Parking management systems</li>
        <li>Toll booth automation</li>
        <li>Vehicle access control</li>
    </ul>

<h2>Contributing</h2>
    <p>
        We welcome contributions! Please fork the repository and submit a pull request with your changes or enhancements.
    </p>

<h2>License</h2>
    <p>
        This project is licensed under the MIT License. See <code>LICENSE</code> for more details.
    </p>
</body>
</html>
