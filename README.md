# Canny Edge Detection

## Aim
To detect edges in an image using the Canny Edge Detection algorithm with OpenCV.

## Requirements
- Python
- OpenCV
- Matplotlib

## Program

```python
import cv2
import matplotlib.pyplot as plt

img = cv2.imread('Image.png', cv2.IMREAD_GRAYSCALE)

blurred = cv2.GaussianBlur(img, (5, 5), 0)

edges = cv2.Canny(blurred, 50, 150)

plt.figure(figsize=(10, 5))

plt.subplot(121)
plt.imshow(img, cmap='gray')
plt.title('Original Image')
plt.axis('off')

plt.subplot(122)
plt.imshow(edges, cmap='gray')
plt.title('Detected Edges')
plt.axis('off')

plt.show()
```

## Output
<img width="970" height="588" alt="image" src="https://github.com/user-attachments/assets/ca25ecb9-e5a5-4bff-bb9a-d9ca22e7aa14" />

## Result
Thus, edges in the given image were successfully detected using the Canny Edge Detection algorithm.
