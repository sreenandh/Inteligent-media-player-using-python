# Inteligent-media-player-using-python
Inteligent Media Player which uses hand gestures instead of keyboard and mouse
Here is the working of the hand gestures in the code:

* **No fingers:** When no fingers are detected, the code does nothing.
* **One finger:** When one finger is detected, the code presses the "space" key. This can be used to play/pause a video or audio file.
* **Two fingers:** When two fingers are detected, the code presses the "up" arrow key. This can be used to increase the volume of a video or audio file.
* **Three fingers:** When three fingers are detected, the code presses the "down" arrow key. This can be used to decrease the volume of a video or audio file.
* **Four fingers:** When four fingers are detected, the code presses the "right" arrow key. This can be used to move forward in a video or audio file.

The code uses a convexity defects algorithm to find the number of fingers in the hand. The convexity defects algorithm works by finding the points on the hand contour that are farthest away from the convex hull of the hand. The number of convexity defects is then used to determine the number of fingers in the hand.

For example, if the code detects four convexity defects, it will determine that there are four fingers in the hand. The code will then press the "right" arrow key.

You can change the keyboard shortcuts used by the code by modifying the code. For example, if you want the code to press the "enter" key when one finger is detected, you can change the code as follows:

```
if count_defects == 1:
    p.press("enter")
```

You can also add more hand gestures to the code. For example, you can add a gesture for rewinding a video or audio file. To do this, you would need to add a new case to the if statement in the code. For example, the following code would add a gesture for rewinding a video:

```
if count_defects == 5:
    p.press("left")
```

Once you have made the changes to the code, you can run it again and the new hand gestures will be detected.
