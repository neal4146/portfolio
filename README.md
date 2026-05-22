# Neal Mehta — Portfolio

> Mechanical Engineering @ Virginia Tech · CS minor · Junior
> <br>Robotics, autonomy, hardware/software intersection. 

📫 [LinkedIn](www.linkedin.com/in/nealmehta12) · nealmehta2005@gmail.com

---

## Team & Research Projects

*Code/CAD owned by the respective teams — writeups + my contributions below.*

### ARGUS — Subsea Inspection ROV
**Role:** CAD Lead · **Team:** ARGUS · **Tools:** SolidWorks, Siemens NX

ARGUS (Advanced Reconnaissance & General Underwater System) is a portable, tethered underwater ROV built for inspecting damaged subsea infrastructure — offshore rigs, pipelines, undersea communication cables — and providing visual reconnaissance for repair assistance.

The pitch: existing inspection solutions are massive, expensive, and require specialized operators. ARGUS is designed to be **portable, easy to deploy, and operable with minimal training** — so a small field crew can show up to a damaged site, drop the ROV in, and get eyes on the problem fast.

**Project status:** Early design phase — currently iterating on individual subsystem components before moving to full assembly.

**Design priorities:**
- **Portable** — small enough for a small team to transport and deploy without a crane or dedicated vessel
- **Wired (for now)** — tethered for reliable power and real-time video; future iterations may move toward autonomy
- **Easy to operate** — minimal training required, simple control interface so the focus stays on the inspection, not the vehicle
- **Modular payload** — swap inspection tools (cameras, sensors) for different mission types

**What I'm working on (CAD lead):**
- Designing the frame, pressure housing, thruster mounts, and buoyancy/ballast subsystems in SolidWorks
- Iterating on individual parts before locking down the full assembly
- Specified Blue Robotics T200 thrusters and integrating them into the buoyancy model toward neutral trim
- Authored the project BOM memo

**Engineering challenges we're working through:**
- Pressure-resistant housing — pressure scales as ~depth², so the housing geometry and seals matter a lot
- Modular payload architecture so the platform can carry different inspection tools without major rework
- Reliable tether communication in deep-water environments

![ARGUS expo poster](images/argus_poster.jpg)

*Project poster from VT Engineering Expo — ARGUS team: Luke Moore, Neal Mehta, Evan Berwick. Advisor: Nathan Li.*

---

### VT Humanoid Robotics — Bipedal Locomotion
**Role:** Controls Sub-team · **Tools:** NVIDIA Isaac Lab, SolidWorks, Python, Reinforcement Learning

VT Humanoid Robotics is a student-led project building a ~3-foot bipedal humanoid from the ground up — mechanical design, electronics, and the controls stack that makes it actually walk. I'm on the controls sub-team, working on the reinforcement learning pipeline that trains walking policies in simulation before deploying them to the real robot.

**The big picture:**
Bipedal walking is one of the hardest control problems in robotics — a humanoid is an inherently unstable system that has to balance itself dozens of times per second across uneven terrain, varying loads, and sensor noise. Classical control gets you partway there; RL lets the robot learn gait strategies that would be nearly impossible to hand-engineer.

**What I'm working on (controls sub-team):**
- **Training RL policies in NVIDIA Isaac Lab** for bipedal locomotion — running massively parallel simulations to train walking policies orders of magnitude faster than real-world training
- **Tuning reward functions** for gait stability, energy efficiency, and trajectory tracking — small changes here can make the difference between a robot that walks and one that face-plants
- **Adapting reference policies** (e.g. the Berkeley humanoid repo) to match our specific robot's URDF and joint configurations
- **Sim-to-real transfer** — building sim environments with domain randomization (varying mass, friction, motor latency) so policies trained in sim actually work on the physical robot
- **URDF / kinematic analysis** of the robot for accurate sim setup

**Engineering challenges:**
- **The sim-to-real gap** — simulation is never perfectly accurate, so a policy that walks beautifully in Isaac Lab often falls flat on real hardware. Domain randomization is the main lever we have to close that gap.
- **Reward shaping** — too sparse and the policy never learns; too dense and it learns to game the reward instead of actually walking. Iterative tuning is most of the work.
- **Real-time control loop** — integrating real sensor feedback (IMU, joint encoders) into the policy at the rates needed for stable balance.

**The robot:**

<p align="center">
  <img src="images/robot.png" width="60%" />
</p>

**Subsystem breakdown — CAD:**

<table>
  <tr>
    <td align="center"><img src="images/torso.png" width="100%" /><br/><sub>Torso</sub></td>
    <td align="center"><img src="images/pelvis.png" width="100%" /><br/><sub>Pelvis</sub></td>
    <td align="center"><img src="images/foot.png" width="100%" /><br/><sub>Foot</sub></td>
  </tr>
</table>

**The team:**

<p align="center">
  <img src="images/HR_team.png" width="70%" />
</p>
---

### SecurITe — ML/AI Security Intern (Summer 2026)
**Role:** ML/AI Security Intern · **Location:** Santa Clara, CA (Remote) · **Dates:** June–August 2026 · 🔗 [securite.world](https://securite.world/)

<img src="images/securite.png" width="200" />

Working on rogue AI agent detection at a cybersecurity company focused on ML/AI security.

*Details limited due to NDA.*

---

## 🔧 Personal Builds

*Full repos on my profile — click through for BOMs, build logs, and photos.*

### 🛸 [Racing Drone](https://github.com/neal4146/racing-drone)
Custom 5" racing quad. Frame to firmware. Currently in config + flashing phase.
**Stack:** iFlight XING-E Pro 2207, SoloGood F722, ELRS, Betaflight

### 🚲 Motorized Bicycle *(repo coming soon)*
Conversion build — adding a motor to a standard bicycle.

### 🐕 SpotMicro Quadruped *(planned)*
Open-source quadruped robot build. On the to-do list.

---

## 🎓 Background

**Virginia Tech** — B.S. Mechanical Engineering, CS Minor · Expected May 2028
Transferred from Manipal Institute of Technology after one year of CS.

**Previously:**
- Data analysis + frontend dev intern @ AgeMates (healthcare nonprofit, Pune)
- Co-authored research paper on senior healthcare tech — published through the Asiatic Society of Mumbai

---

## 📫 Contact

- LinkedIn: [Neal Mehta](www.linkedin.com/in/nealmehta12)
- Email: nealmehta2005@gmail.com
- GitHub: [neal4146](https://github.com/neal4146)