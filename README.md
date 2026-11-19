# FormVision

A push-up counter needs to recognize a full return to the starting position. The notebook measures the left shoulder–elbow–wrist angle in the image, enters the down state below 120°, then adds one rep when the angle exceeds 175°. Frames between those thresholds leave the count alone. Compare the [input clip](pushups/pushup_video.mp4), [annotated clip](pushups/annotated_output.mp4) and [counter implementation](pushups/Pushup%20counter.ipynb).

The camera is part of this measurement. A change in viewpoint changes the projected elbow angle, and a missing pose can hide a transition. The clips demonstrate what the overlay displays for these recordings. A claim about counting accuracy would require independently labeled repetitions across people and camera positions.

The other folders contain examples for [squats](Squats/Squats%20counter.ipynb), [bench press](Bench%20press/bench%20press.ipynb), [deadlift](deadlift/deadlift%20counter.ipynb), [plank holds](plank%20hold/plank.ipynb), [one-leg balance](one%20leg%20balance/one%20leg%20balance.ipynb), [hamstring flexibility](hamstring%20stretch/hamstring_stretch.ipynb) and [shoulder flexibility](shoulder%20stretch/shoulder_stretch.ipynb). Open each notebook from its exercise folder so its video filename resolves. The push-up notebook uses OpenCV, the MediaPipe `solutions.pose` API, NumPy, Matplotlib and IPython.

