# MultiStream-Connect
MultiStream Connect is a client-server application for real-time video streaming with concurrent client support. It uses multithreading for efficient management and features a user-friendly GUI with Tkinter. Capture, serialize, and display video frames using OpenCV.

Key Features

Save Local Transfer:

Since the server and client are both on a local network, anyone without access to the network cannot interfere with data. Furthermore, processing is kept on server side so client side code can be run on micro controllers on IOT devices(Smart Cameras) without issue and processing can be done on a more resource heavy server side PC.

Client-Server Communication:

Establishes TCP connections using Python's socket library.
Handles multiple clients concurrently with threading.
Streams video frames from clients to the server.
Video Streaming:

Captures video frames using OpenCV and resizes them with imutils.
Serializes video frames with pickle for network transmission.
Displays video frames in real-time on the server.
Multithreading:

Manages multiple clients in parallel using threads for efficient performance.
GUI Integration:

Implements a Tkinter GUI for both the server and client applications.
Server GUI for monitoring and managing connected clients.
Client GUI for starting, stopping, and disconnecting the video stream.
Client Management:

Uses a dictionary to track connected clients.
Supports client termination when necessary, ensuring smooth server operation.


python server.py
python client.py
