# butterfly_detection

1. Download the videos with different resolution by using library pytube. Simply download the video with the highest resolution.
   
2. Load pre-trained model for detection by opencv and 'Yolov3' is used.

3. Capture each frame of the video and find out frame per second.

4. Read the frame and input and frame to yolo model for obeject detection. Assign the position of bufferflies as box. (Yolo model did not train for butterfly and the class id == 56 in my code is not true, that's why the code doesn't work)

5. If there is butterfly detected, add a tracker object to track its movement, count the number of tracker(s) of a frame and print the number of tracked butterflies.

6. If the tracker box was out of frame, it indicate that the butterfly is flying away and out of frame.

7. Store the result frame and output as a new video.
   
   
