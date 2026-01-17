# SKY MISSIONS: Machine Learning & Game Development

**Sky Missions** is an advanced 3D drone simulation developed in Unity. It features a drone trained using **Reinforcement Learning** to navigate complex environments, avoid obstacles, and execute mission protocols autonomously.

---

## 🎮 Download & Play
To download the game, click the link for your OS and then click the **"View Raw"** button on the next page.

* **[Download for Windows](https://github.com/hadirida46/SKY-MISSIONS/raw/main/SKY_MISSIONS_Windows.zip)**
* **[Download for Linux](https://github.com/hadirida46/SKY-MISSIONS/raw/main/SKY%20MISIONS%20For%20Linux.tar.gz)**

---

## 📄 Project Documentation & Resources
For a deep dive into the math, training process, and project architecture, refer to the following:

* 📑 **[Project Report (PDF)](https://github.com/hadirida46/SKY-MISSIONS/raw/main/SKY-MISSIONS-Report.pdf)**
* 📊 **[Presentation Slides (PDF)](https://github.com/hadirida46/SKY-MISSIONS/raw/main/SKY-MISSIONS-Slides.pdf)**
* 📈 **[Training Logs & Summaries](https://github.com/hadirida46/SKY-MISSIONS/tree/main/logs_summary)**

---

##  Main Menu
![Main Menu](screenshots/Main%20Menu.png)

---

## 🕹️ Missions

### 01 – Building Strike (Manual Control)
* **Purpose:** Compare human control against AI behavior.
* **Flow:** Navigate the drone into a building and deploy the payload manually.
* **Controls:** Use **WASD** to fly.

![Mission 1](screenshots/Building%20Strike.png)

---

### 02 – Building Strike (AI Assist)
* **Purpose:** Autonomous drone strike with AI navigation.
* **Flow:** Drone starts camouflaged, flies to target, strikes, and returns home.
* **Controls:** * `1` or `2`: Select Target Building
    * `H`: Return to Home

![Mission 2](screenshots/Building%20Strike%20(AI%20assist).png)

---

### 03 – Vehicle Hunter (AI Assist)
* **Purpose:** Target tracking of a moving vehicle.
* **Flow:** Drone tracks the vehicle autonomously and triggers an engagement sequence.
* **Controls:** * `C`: Command chase
    * `A`: Trigger attack

![Mission 3](screenshots/Vehicle%20Hunter.png)

---

### 04 – Control Vehicle (Avoid Drone)
* **Purpose:** Evasion scenario against an AI drone.
* **Flow:** You drive the vehicle; the AI drone hunts you.
* **Controls:** **WASD** to drive the vehicle.

![Mission 4](screenshots/Avoid%20Drone.png)

---

## 🧠 Technical Overview
* **Algorithm:** Proximal Policy Optimization (PPO) via Unity ML-Agents.
* **Sensing:** Sphere-based detection for 360-degree obstacle awareness.
* **Training Logic:** We used **Reward Shaping** to solve "Catastrophic Forgetting," where the drone would prioritize avoiding obstacles over its mission.
