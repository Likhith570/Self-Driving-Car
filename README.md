This project deals with  a Computer Vision Pipeline designed to detect objects and process video frames for self-driving simulation.
The script follows a standard "Process-Loop" architecture:

Configuration: It identifies system paths to pre-trained detection models (Haarcascades) using cv2.data.haarcascades.

Ingestion: It uses cv2.VideoCapture to load video files or streams into memory.

The Loop: A while loop continuously executes:

Frame Capture: play.read() extracts a single image frame from the video.

Processing: It applies detection logic to identify objects within that frame.

Visualization: cv2.imshow() renders the frame in a window so you can see the results in real-time.
Exit Control: It listens for the 'q' key to stop the loop, then releases the video resources
