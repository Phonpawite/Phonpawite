import matplotlib.pyplot as plt

# กำหนดตำแหน่งของจรวดและดวงจันทร์
rocket_position = [0, 0]  # ตำแหน่งจรวด [x, y]
moon_position = [0, 0]    # ตำแหน่งดวงจันทร์ [x, y]

# พล็อตจรวดและดวงจันทร์
plt.plot(rocket_position[0], rocket_position[1], 'ro', label='Rocket')
plt.plot(moon_position[0], moon_position[1], 'bo', label='Moon')

# เพิ่มเส้นที่เชื่อมระหว่างจรวดและดวงจันทร์
plt.plot([rocket_position[0], moon_position[0]], [rocket_position[1], moon_position[1]], 'k--')

# ตั้งค่าแกน x และ y
plt.xlabel('X')
plt.ylabel('Y')

# เพิ่มชื่อเรื่องและคำอธิบาย
plt.title('Rocket on the Moon')
plt.legend()

# แสดงกราฟ
plt.grid(True)
plt.axis('equal')  # ทำให้มุมมองในรูปเท่ากัน

plt.show()
