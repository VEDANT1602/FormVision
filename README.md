# FormVision

Watch the elbow angle in the [annotated push-up clip](pushups/annotated_output.mp4). A rep counts on the way back up. Bending the left elbow past the down threshold (below 120°) arms the counter. Extending it above 175° adds one rep and resets the state. Staying at the top for several frames still counts once. [Original clip](pushups/pushup_video.mp4) · [Counter notebook](pushups/Pushup%20counter.ipynb)

The angle comes from the shoulder, elbow and wrist projected onto the image. Move the camera and the same movement can cross a different threshold. These recordings show how the overlay behaves. Measuring rep-count accuracy would take separately labeled repetitions across people and camera positions.

The other folders contain examples for [squats](Squats/Squats%20counter.ipynb), [bench press](Bench%20press/bench%20press.ipynb), [deadlift](deadlift/deadlift%20counter.ipynb), [plank holds](plank%20hold/plank.ipynb), [one-leg balance](one%20leg%20balance/one%20leg%20balance.ipynb), [hamstring flexibility](hamstring%20stretch/hamstring_stretch.ipynb) and [shoulder flexibility](shoulder%20stretch/shoulder_stretch.ipynb). Open each notebook from its exercise folder so its video filename resolves. The push-up notebook uses OpenCV, the MediaPipe `solutions.pose` API, NumPy, Matplotlib and IPython.

