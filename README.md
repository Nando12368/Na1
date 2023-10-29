import turtle as t

# Fungsi untuk menggambar hati
def draw_heart():
    t.begin_fill()
    t.fillcolor('#FF1493')  # Warna merah muda
    t.left(140)
    t.forward(224)
    for _ in range(200):
        t.right(1)
        t.forward(2)
    t.left(120)
    for _ in range(200):
        t.right(1)
        t.forward(2)
    t.forward(224)
    t.end_fill()

# Fungsi untuk menulis teks "I Love You"
def write_text():
    t.penup()
    t.goto(0, -250)  # Posisi teks di bawah hati
    t.pendown()
    t.color('#FF1493')  # Warna teks
    t.write("I Love You", align="center", font=("Arial", 24, "normal"))

# Konfigurasi turtle
t.speed(0)
t.bgcolor('black')  # Warna latar belakang

# Gambar hati
draw_heart()

# Tulis teks
write_text()

t.hideturtle()
t.done()
