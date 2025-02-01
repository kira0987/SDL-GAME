# 🏰 Medieval Enigma: The Hero's Quest

## 📌 Project Overview

**Medieval Enigma: The Hero's Quest** is a **2D puzzle-platformer game** developed using the **SDL framework** in C. The game is set in a **mystical medieval castle**, where the player takes on the role of a brave hero on a mission to rescue a princess. Throughout the journey, the hero must overcome **challenging enigmas, deadly obstacles, enemy encounters, and lava-filled paths** to reach the final chamber where the princess is held captive.

This game was developed as a **first-year Computer Science Engineering project** at **ESPRIT University**, in collaboration with **Oussema Assal**. The project took **4 years** to refine but was never properly committed due to a lack of expertise in Git at the time.

🎵 The **World of Warcraft theme song** is used as the background music, enhancing the immersive medieval experience.

---

## 🎮 Gameplay Features

✔ **Hero’s Journey:** Explore a vast medieval castle full of puzzles and obstacles.
✔ **Enemies & Traps:** Dodge dangerous enemies and avoid timed obstacles.
✔ **Lava Pits & Platforms:** Navigate treacherous castle floors with precision jumps.
✔ **Enigmas & Puzzles:** Solve intricate puzzles to unlock pathways.
✔ **Epic Soundtrack:** Feel the atmosphere with the World of Warcraft theme.

---

## 🛠 Installation & Execution

### **📌 Prerequisites**

Before running the game, ensure you have the required SDL libraries installed:

```sh
sudo apt-get install libsdl1.2-dev libsdl-image1.2-dev libsdl-ttf2.0-dev libsdl-mixer1.2-dev
```

### **▶ Running the Game**

The game is built using a **Makefile**, which simplifies the compilation process. To run the game, execute the following commands in your terminal:

```sh
make
./test.exe
```

This will compile the game and launch the executable directly.

---

## 🔥 Makefile Configuration

The Makefile used for compiling and running the game is structured as follows:

```makefile
prog: image.o test.o text.o Settings.o background.o perso.o personnage.o enigme_image.o ennemi.o
	gcc test.o image.o text.o Settings.o background.o perso.o personnage.o enigme_image.o ennemi.o -o test.exe -lSDL -lSDL_image -lSDL_ttf -lSDL_mixer

test.o: test.c
	gcc -c test.c -g

image.o: image.c
	gcc -c image.c -g

text.o: text.c
	gcc -c text.c -g

Settings.o: Settings.c
	gcc -c Settings.c -g

background.o: background.c
	gcc -c background.c -g

perso.o: perso.c
	gcc -c perso.c -g

personnage.o: personnage.c
	gcc -c personnage.c -g

enigme_image.o: enigme_image.c
	gcc -c enigme_image.c -g

ennemi.o: ennemi.c
	gcc -c ennemi.c -g
```

Executing `make` will compile all necessary game files, and `./test.exe` will launch the game.

---

## 🎥 Visual Preview

### **Gameplay Video** 🎬



### **Screenshots** 📸

| Hero in Action |      Traps      | The Castle |
| -------------- | --------------- | ---------- |
|                |                 |      https://github.com/kira0987/SDL-GAME/blob/main/background/test.jpg      |

---

## 🤝 Contributing

Contributions are welcome! Follow these steps:

1. **Fork the repository**
2. **Create a new branch** (`git checkout -b feature-branch`)
3. **Make your changes and commit** (`git commit -m "Added new feature"`)
4. **Push your branch** (`git push origin feature-branch`)
5. **Open a Pull Request**

---

## 📜 License

This project is **open-source** and follows the **MIT License**.

---

### 💡 **Follow & Support**

🔹 **GitHub:** [Houssam eddine Ben Kheder](https://github.com/kira0987)\
🔹 **University:** ESPRIT - 1st Year Computer Science Engineering

🚀 **Embark on the quest, defeat the enemies, and rescue the princess!** 🏰



