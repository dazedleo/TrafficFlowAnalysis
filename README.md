Welcome to the Traffic Flow Analysis project!
This Python-based solution lets you automatically count vehicles in three different lanes by applying state-of-the-art computer vision to a real traffic video—no manual labeling, no external tools needed.

Overview
This tool downloads a public YouTube traffic video and analyzes it frame-by-frame:

Detects and tracks cars, buses, and trucks

Defines lane boundaries and assigns detected vehicles to lanes

Counts vehicles per lane and prevents double-counting

Exports results to CSV and overlays visuals on the processed video

Features
Automated video download: Just run the script—no need to manually download the video.

Vehicle detection: Uses a pre-trained YOLO (COCO weights) for robust detection.

Multi-object tracking: Sorts and follows each vehicle through the frames.

Custom lane regions: Easily adjustable lane definitions for any road layout.

Real-time processing: Designed to run smoothly on standard hardware.

Visual overlays: See counts and lanes directly on the video.

Results export: Get a CSV log with vehicle IDs, lane numbers, frame counts, and timestamps.

Quick Start
1. Clone the repository:

bash
git clone https://github.com/yourusername/traffic-flow-analysis.git
cd traffic-flow-analysis
2. Install Python dependencies:

bash
pip install -r requirements.txt
You may also need to install ffmpeg for video handling. See ffmpeg.org for installers.

3. Run the script:

bash
python traffic_flow.py
4. Watch the lanes fill with live counts, and check vehicle_detection_log.csv for detailed results.

Output
A video showing live lane counts and tracking boxes.

A CSV with vehicle ID, lane, frame, and timestamp data.

A console summary of total vehicles per lane.

