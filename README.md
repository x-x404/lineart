# ✏️ LineArt for Blender 4.x

**LineArt** is a stylized line generation system for **Blender 4.x**, designed to create **hand-drawn–like line art** quickly and efficiently.
It is ideal for **NPR / toon-style rendering**, illustrations, and stylized shading workflows.

The system is built using **Geometry Nodes** and **Material Nodes**, allowing flexible control and real-time preview directly in the viewport.

---

## 🔧 Requirements

Before using LineArt, make sure you have:

* **Blender 4.0+**
* **EEVEE Render Engine**
  ⚠️ Cycles is technically supported, but **not recommended** due to potential unexpected artifacts
* **LSPotato Addon** Download at [HERE](https://github.com/lvoxx/LSPotato)

---

## 📥 Installation

There are **two ways** to install LineArt:

### **Method 1: Clone / Download**

* Clone this repository or download the **latest release**
* Append the following node groups into your project:

  * `Line Art Geo`
  * `LA: Add Line Art`
* Use them as standard Geometry Nodes

---

### **Method 2: LSRegistry (Recommended)**

* Open the **LSPotato** addon
* Go to **LSRegistry**
* Add the following entry to the registry list:

  ```
  io.github.x-x404.lineart:0.0.1
  ```
* Download and install automatically

---

## 🚀 Usage Guide

### **1️⃣ Add Geometry Nodes**

* Add a **Geometry Nodes modifier** to the object that will *draw* the lines
* ⚠️ This is **not** the object being outlined
* You can use an **Empty object** or any mesh as the line drawer

<img alt="Step 1" src="assets\1.png" width="800px" height="auto"/>

---

### **2️⃣ Create LineArt Material**

* Create a new material for line art
* Connect the **`LA: Add Line Art`** node to **Material Output**
* Enable the following settings:

  * **Camera Backface Culling**
  * **Shadow Backface Culling**
  * Blend Mode: **Blended**

<img alt="Step 2" src="assets\2.png" width="800px" height="auto"/>

---

### **3️⃣ Assign Scene & Camera**

* Specify:

  * The **scene** to generate line art from
  * Objects to **exclude** from line generation
* Select **one main camera** for the scene

<img alt="Step 3" src="assets\3.png" width="400px" height="auto"/>

### **4️⃣ Result**

<img alt="Result" src="assets\4.png" width="800px" height="auto"/>

---

## 🧩 Notes

* Optimized for **NPR / toon workflows**
* Works best with **EEVEE**
* Can be combined with other stylized shaders in the **LSCherry ecosystem**

---

## 🐞 Support & Feedback

* Join the **LSCherry Discord** for direct support
* Or create an **Issue** in this repository to report bugs or request features

---

If you want, I can also:

* Write **release notes** for GitHub Releases
* Create a **short showcase description**
* Or prepare **multi-language versions (JP / CN)**
