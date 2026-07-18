# 🚗 Tesla Predictive Drive Assist v6.1 (Jailbreak Mod)

> Real-time raycast steering assist  
> NOT autonomous — full manual control always

---

## ⚙️ Overview

Tesla Predictive Drive Assist is a raycast-based driver assist system.

- Up to **100 raycasts**
- Real-time path calculation (every frame)
- Collision avoidance
- Automatic centering
- Fully manual steering preserved

---

## 🧠 Raycast System

- Rays project forward in a spread pattern
- Dynamically adjust based on steering
- Continuously scan environment

---

## 🎯 Ray States

- 🟢 **GREEN** → Safe path  
- 🟡 **YELLOW** → Wall detected, no collision  
- 🟠 **ORANGE** → Near collision  
- 🔴 **RED** → Immediate collision  

---

## 📐 Adaptive Behavior

**Driving straight**
- Forward rays extend
- Side rays widen

**Turning**
- Rays extend toward turn direction
- Opposite rays shorten
- Forward rays slightly shorten

All transitions are smoothed.

---

## 📊 Confidence System

- Rays split into **left / right**
- Each side calculates **% of GREEN rays**

**Logic:**
- More GREEN on one side → steer that way  
- Equal → no correction  

---

## 🧱 Collision Avoidance

- ORANGE / RED increase steering strength
- Immediate danger overrides centering

---

## 🧭 Centering

- When both sides are safe:
  - System balances steering
  - Keeps vehicle centered (e.g. tunnels)

---

## ✋ Manual Override

- Any steering input = assist pauses instantly
- No resistance
- Auto-resumes when input stops

---

## 🎮 Steering Output

- Smoothed turning
- No abrupt movement
- Strength based on:
  - Ray urgency
  - Confidence level

---

## ⚡ Performance

- Runs every frame
- Optimized ray processing
- Stable at max ray count

---

## ✅ Summary

- Non-autonomous assist
- Raycast-based environment detection
- Confidence-driven steering
- Collision avoidance
- Full driver control at all times



## 🛠️ How to Use

### 1. Spawn Vehicle
- Spawn a supported car in-game

---

### 2. Connect the System
- Click on the car model (ModelClick / interaction prompt)
- The system will attach to the vehicle

---

### 3. Enter the Vehicle
- Sit in the driver seat as normal

---

### 4. Enable Drive Assist
- Locate the **Drive Assist** control
- Toggle it ON

---

### 5. Drive

- Steering remains fully manual
- Assist will:
  - Analyze surroundings in real time
  - Help avoid collisions
  - Keep the vehicle centered when possible

---

### ⚙️ Settings & Debug

- Open settings panel to:
  - Adjust behavior
  - Tune responsiveness
  - Modify ray settings

- Enable **Debug Mode** to:
  - View raycasts in real time
  - See color states (GREEN / YELLOW / ORANGE / RED)
  - Monitor system behavior live
