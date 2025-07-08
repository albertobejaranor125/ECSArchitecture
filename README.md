# 🧠 ECS Architecture | C++ Game Systems Simulation

This project is part of my learning path in game development using C++. It implements a lightweight **Entity-Component-System (ECS)** architecture and simulates basic game systems such as animation, input, movement, health, and collision.

The goal is to gain a deeper understanding of **data-driven game architectures**, and how to decouple logic using systems over inheritance.

---

## 🚀 Features

- ✅ **ECS Design**: Entities, Components, and Systems are cleanly separated
- 🎯 **Component-based logic**: Plug-in behaviors per entity
- ⚙️ **Systems implemented**:
  - `MovementSystem`: Moves entities with `Position`
  - `HealthSystem`: Reduces HP over time
  - `AnimationSystem`: Updates animations frame by frame
  - `InputSystem`: Simulates player commands (idle, move, attack)
  - `DeathSystem`: Logs when an entity dies
  - `CollisionSystem`: Detects basic AABB collisions
  - `LoggerSystem`: Logs activity to console and file (`log.txt`)

---

## 🧩 Components Used

| Component   | Description                           |
|-------------|---------------------------------------|
| `Position`  | Stores x/y coordinates                |
| `Health`    | Manages current and max HP            |
| `Name`      | Identifier for the entity             |
| `Animation` | Tracks animation state and frame time |
| `Input`     | Holds last player input command       |
| `Collider`  | Axis-aligned bounding box for entity  |

---

## 🛠️ How to Build

### Requirements
- C++11 or higher
- Compatible compiler (G++, Clang, MSVC)

### Compile and Run
```bash
g++ -std=c++11 -o ECSGame main.cpp
./ECSGame
