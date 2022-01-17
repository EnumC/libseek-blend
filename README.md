# libseek-blend
SEEK Thermal Imager viewer program with real-time thermal visible image blending support.

This project is designed to create a full-fledged UI for the SEEK thermal camera. 

## Supported Features:
- [ ] Real-time image blending (similar to MSX or SeekFusion)
- [ ] Alignment calibration
- [ ] Adjustable palette selection
- [ ] Large touch targets

The image blending can be accomplished by performing image registration. We can implement this using ORB in order to find relevant keypoints and descriptors. Then, we compute the homography using the previous data and transform the visible image's perspective. This provides us with a visible image that can be overlaid on the IR image. We can further improve this feature by using contour detection on the visible image in order to only display outline of objects. 

The FPS degradation and latency will need to be tested in order to determine feasability and usability. 

## Thanks To
The following projects that made this possible:

* https://github.com/OpenThermal/libseek-thermal
* https://github.com/opencv/opencv

## Additional Resources

