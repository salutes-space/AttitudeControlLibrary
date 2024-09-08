# 🚀 Attitude Control Library 🚀 

Welcome to your go-to library for mastering **attitude control** by exploring the Attitude Math Library (**AML**) in C++! Whether you're an aerospace engineer looking to fine-tune satellite orientation, a computer vision specialist working on 3D transformations, or a game developer creating immersive worlds, **AML** will equip you with the tools to understand and apply **attitude mathematics** in real-world applications! 🌍

---

## Why Learn Attitude Control? 🤔

### Aerospace Engineers 🛰️
For satellites, rockets, and spacecraft, precise **attitude control** is essential for maintaining proper orientation. Understanding quaternions, DCMs, and Euler angles means mastering the science of navigating the stars!

### Computer Vision Engineers 📷
In computer vision, rotations and transformations are crucial for accurate 3D modeling and object recognition. AML's vector and matrix tools will help handle complex rotations with ease!

### Game Developers 🎮
Game physics, camera controls, and 3D models all rely on attitude control. Master AML to take full control of object orientation and create fluid, realistic experiences for players!

---

## Project Overview

AML provides a powerful, easy-to-use C++ library for performing 3D attitude calculations, such as quaternion operations, DCMs, and more. **Master the math behind rotation** and become proficient in your field!

---

## 🚀 Getting Started

### Requirements
- **CMake** (version 3.15+)
- A C++ compiler (standard 11)

### Build & Run

1. **Configure the project**:
   ```bash
   cmake -S . -B app
   ```

2. **Build the project**:
   ```bash
   cmake --build app
   ```
   🛠️ Find examples in the `app/example/AML_Example` folder!

3. **Run Tests**:
   ```bash
   ctest --test-dir app
   ```
   🧪 Ensure everything works perfectly with built-in tests!

---

## 📂 Project Structure

```plaintext
AttitudeMathLib/
├── AML/
│   ├── AML.h
│   ├── AMLDCM.cpp
│   ├── AMLDCM.h
│   ├── AMLEulerAngles.cpp
│   ├── AMLEulerAngles.h
│   ├── AMLMatrix33.cpp
│   ├── AMLMatrix33.h
│   ├── AMLQuaternion.cpp
│   ├── AMLQuaternion.h
│   ├── AMLVector3.cpp
│   ├── AMLVector3.h
│   └── CMakeLists.txt
├── example/
│   ├── CMakeLists.txt
│   └── main.cpp
└── test/
    ├── AMLDCMTest.cpp
    ├── AMLMatrix33Test.cpp
    ├── AMLVector3Test.cpp
    ├── CMakeLists.txt
    ├── catch/
    │   └── catch.hpp
    └── main.cpp
```

### **AML/ Folder** 📐
- **AMLDCM.cpp & .h**: 🌐 Rotation transformations using Direction Cosine Matrices (DCM).
- **AMLEulerAngles.cpp & .h**: 📏 Euler angles and their role in attitude calculations.
- **AMLMatrix33.cpp & .h**: 🧮 Matrix operations for 3x3 matrices.
- **AMLQuaternion.cpp & .h**: ✨ Quaternion operations for smooth 3D rotations.
- **AMLVector3.cpp & .h**: 📊 3D vector operations.

### **example/ Folder** 🛠️
- **main.cpp**: A simple program demonstrating how AML handles attitude transformations in real-world applications.

### **test/ Folder** 🧪
- **AMLDCMTest.cpp**: Unit tests for DCM operations.
- **AMLMatrix33Test.cpp**: Unit tests for matrix operations.
- **AMLVector3Test.cpp**: Unit tests for vector operations.
- **catch.hpp**: Catch2 testing framework for easy and effective testing.

### **CMakeLists.txt**
The CMake configuration to build everything seamlessly.

---

## ⚖️ Comparison of Attitude Representations

| Representation | Advantages                                  | Disadvantages                                           |
|----------------|---------------------------------------------|--------------------------------------------------------|
| **DCM (Direction Cosine Matrix)** | 🌍 Intuitive and easily interpretable <br> 🌐 Direct transformation matrix | 🧮 Requires 9 elements <br> 🚨 Numerical drift over time without orthogonalization |
| **Euler Angles** | 🎯 Simple and intuitive for basic 3D orientations <br> 🔧 Easy to use in basic systems | 🚧 Gimbal lock problem <br> ⏳ Not suitable for continuous rotations |
| **Quaternions** | ⚡️ Compact (only 4 elements) <br> 🔄 No gimbal lock <br> 🔥 Smooth interpolation (slerp) | 🛠 Harder to visualize <br> 🧩 Requires normalization to avoid errors |
| **Axis-Angle** | 🌐 Minimal representation (only 3 elements) | 🧮 Conversion required for complex operations <br> 🔄 Interpolation more complex than quaternions |

---

## 🛡️ Safety and Scalability

**AML** is designed to be easy to use and efficient for both **research and development**, and for direct integration with **embedded systems** and **microprocessors** used in **satellites**, **UAVs**, or even **reusable rocketry**! 🚀 The lightweight and modular design makes it ideal for real-world aerospace applications.

### A Few Suggestions for Safety-Critical Systems:
- **Dynamic Memory Allocation (DMA)**: Implementing DMA will help manage memory efficiently, crucial for environments with limited resources.
- **Virtual Classes**: Using virtual classes to implement polymorphism enhances code extensibility and maintainability, making it more robust for complex systems.

---

## 🧠 Powered by **Chirb.com**

This library was prepared and integrated with the help of **Chirb**, the cutting-edge AI assistant tool from **Salutes Space Germany**. Chirb offers seamless integration with development and embedded machines, making the process smooth and intuitive. **Chirb** is a unique AI assistant that not only helps in code preparation but can also integrate directly with embedded systems for testing, optimization, and deployment! 🛰️

---

## 🌟 Conclusion

Whether you're designing cutting-edge satellites, fine-tuning UAVs, or pioneering the future of reusable rocketry, **Attitude Control Library** offers the tools you need to master attitude control. This **C++ library** is **optimal for research and development**, and it's designed to integrate seamlessly with **embedded systems**.

**Take control of your project’s orientation—unlock the power of AML and launch your next breakthrough! 🚀**

---

## 📝 License

This project is distributed under the **MIT License**, giving you freedom to use, modify, and distribute the software. You can find the full license in the `LICENSE` file.

Refereces:
<div><p style="line-height: 1.3;text-indent:-34px;margin-left:34px;margin-top:0px;margin-bottom:0em;word-break:break-word;">Dumble, Steven J., and Peter W. Gibbens. 2015. “Airborne Vision-Aided Navigation Using Road Intersection Features.” <i>Journal of Intelligent &#38; Robotic Systems</i> 78 (2): 185–204.</p></div>

<div><p style="line-height: 1.3;text-indent:-34px;margin-left:34px;margin-top:0px;margin-bottom:0em;word-break:break-word;">Gupta, Yadunath, Pulak Halder, and Siddhartha Mukhopadhyay. 2014. “Modeling of Flexible Tactical Aerospace Vehicle for Hardware-in-Loop Simulations.” In <i>Special Topics in Structural Dynamics, Volume 6</i>, 379–99. Conference Proceedings of the Society for Experimental Mechanics. Cham: Springer International Publishing.</p></div>

<div><p style="line-height: 1.3;text-indent:-34px;margin-left:34px;margin-top:0px;margin-bottom:0em;word-break:break-word;">Dumble, Steven J., and Peter W. Gibbens. 2012. “Horizon Profile Detection for Attitude Determination.” <i>Journal of Intelligent &#38; Robotic Systems</i> 68 (3–4): 339–57.</p></div>
