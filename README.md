# Data Visualization Using ML Tools
---
```python
plt.plot(x,y, label="Line 1", color="blue", linestyle="--", marker="o")  # Line 1

plt.plot(x,y*2, label="Line 2", color="red", linestyle="-.", marker="s")  # Line 2

plt.plot(x,y*3, label="Line 3", color="green", linestyle="-", marker="D")  # Line 3

plt.title("Three Lines Example")

plt.xlabel("X-Axis")
plt.ylabel("Y-Axis")

plt.legend()

plt.show()
```
<img width="571" height="455" alt="image" src="https://github.com/user-attachments/assets/4371b519-d91e-4f57-a323-eb8ecb4bcbee" />

---
```python

marker_options = [
    "o",  # Circle
    "s",  # Square
    "^",  # Triangle up
    "v",  # Triangle down
    "<",  # Triangle left
    ">",  # Triangle right
    "d",  # Diamond
    "D",  # Thick diamond
    "p",  # Pentagon
    "*",  # Star
    "h",  # Hexagon 1
    "H",  # Hexagon 2
    "+",  # Plus
    "x",  # X (cross)
    ".",  # Point
    ",",  # Pixel
]


```
     
---

x1 = [1, 2, 3, 4, 5]
y_base = [2, 4, 6, 8, 10]

for i, m in enumerate(marker_options):
    plt.plot(x1, [y + i for y in y_base], label=f"Marker {m}", marker=m)

plt.title("Different Marker Options")
plt.legend()
plt.show()

<img width="543" height="435" alt="image" src="https://github.com/user-attachments/assets/e796455b-ed42-4f81-8c3a-23d8b4239c85" />
