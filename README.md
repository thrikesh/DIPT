# DIPT
# ROCKET:
```
import cv2
from matplotlib import pyplot as plt

image = cv2.imread('p2.jpg',cv2.IMREAD_GRAYSCALE)

height, width = image.shape
print("Width:", width)
print("Height:", height)

plt.figure(figsize=[10, 10])
plt.imshow(image, cmap='gray')
plt.axis('off')
plt.show()

image = cv2.imread("p2.jpg")
fig, ax = plt.subplots()
ax.imshow(image)
ax.set_xticks(range(0, image.shape[1], 100))
ax.set_yticks(range(0, image.shape[0], 100))
plt.show()

image = cv2.imread("p2.jpg")
x, y = 500, 50
width = 200
height = 600
cv2.rectangle(image, (x, y), (x + width, y + height), (0, 0, 255), 3)

fig, ax = plt.subplots()
ax.imshow(image)
ax.set_xticks(range(0, image.shape[1], 100))
ax.set_yticks(range(0, image.shape[0], 100))
plt.show()
```
# LAKE:
```
import cv2
import matplotlib.pyplot as plt

image = cv2.imread('p1.jpg', cv2.IMREAD_COLOR)

print("Image shape (color):", image.shape)

gray_image = cv2.cvtColor(image, cv2.COLOR_BGR2GRAY)

print("Image shape (grayscale):", gray_image.shape)

plt.figure(figsize=[10, 10])
plt.imshow(gray_image, cmap='gray')
plt.axis('off')
plt.show()
```

# OUTPUT:
![image](https://github.com/user-attachments/assets/94f0822b-ac3c-4b23-9f4c-d6c89b1d33c7)
![image](https://github.com/user-attachments/assets/efcfba7f-3c3a-4076-96c8-4844bada3d9d)




