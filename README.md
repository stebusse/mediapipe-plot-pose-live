# MediaPipe plot pose live

This little script lets you plot the pose world landmarks from MediaPipe in neat 3D diagram.

<a href="https://drive.google.com/uc?export=view&id=1AKUDIZdfPwNcMWZ1HQK-c7iBknf4Bls1"> <img src="https://drive.google.com/uc?export=view&id=1AKUDIZdfPwNcMWZ1HQK-c7iBknf4Bls1" alt="example plot" width="300"/>
</a>

## Usage

For full usage see `example.py`

```
import plot_pose_live
import matplotlib.pyplot as plt

# create axes like this 
fig = plt.figure()
ax = fig.add_subplot(111, projection="3d")

```
Get your results from the pose estimation in ḾediaPipe
```
# calculate pose
results = pose.process( ...

# draw 3D pose landmarks live
plot_pose_live.plot_world_landmarks(ax, results.pose_world_landmarks)

```