# Sun Pointer ![Sun Pointer UEIcon](Resources/SunPointer_icon32.png)

**Sun Pointer** is an intuitive Editor Utility Widget for Unreal Engine designed to take the guesswork out of lighting your scenes. Instead of wrestling with rotation values or the Directional Light gizmo, Sun Pointer allows you to position your sun visually by "pointing" exactly where you want it to be.

![Sun Pointer UI](Resources/SunPointer_UI.png)

## 🚀 The Concept
The tool uses a **Sun Alignment Dummy** as a visual target. By calculating a vector from your **active viewport camera** through the dummy, the tool places the sun along that same line at a fixed distance. This ensures that the sun appears exactly where you are looking through the dummy, making "hero shot" lighting effortless.

---

## ✨ Key Features

* **Point-and-Shoot Lighting:** Align the sun based on your current perspective.
* **Smart Actor Detection:** The "Find Actors" button automatically scans your scene and links your Directional Light, Sun Sphere, and Dummy.
* **Instant Teleportation:** Use the "Teleport" button to bring the alignment dummy directly in front of your camera, no matter how large the level is.
* **Visibility Controls:** Easily toggle the visibility of the dummy and sun sphere to keep your viewport clean while working.
* **Customizable Distance:** Fine-tune the Sun Sphere scale and distance to clear your far-clip plane or fit your world's atmosphere.

---

## 📖 Quick Start Guide

If you are setting up Sun Pointer for the first time in a level:

1.  **Launch the Tool:** Right-click `EUW_SunPointer` in your Content Browser and select **Run Editor Utility Widget**.
2.  **Spawn Assets:** Click **Spawn Sun Alignment Dummy** and **Spawn Sun Sphere** to add the necessary actors to your Outliner.
3.  **Link Your Scene:** Click **Find Actors**. The tool will automatically populate the Directional Light, Sun Sphere, and Dummy fields.
4.  **Position the Sun:**
    * Fly your viewport camera to your desired vantage point.
    * Click **Teleport Sun Alignment Dummy to Viewport** to bring the target into view.
    * Move the Dummy actor (the sun icon) to the specific spot in the sky where you want the sun.
5.  **Sync:** Hit **Update Sun**. Your light will instantly rotate to match the trajectory from your camera through the dummy.

---

## 🛠 UI Overview

| Button / Field | Function |
| :--- | :--- |
| **Find Actors** | Automatically hooks up the tool to existing light and dummy actors in the scene. |
| **Teleport Dummy** | Snaps the alignment target to a fixed distance in front of your current viewport camera. |
| **Update Sun** | Executes the vector math and snaps the Directional Light and Sun Sphere into alignment. |
| **Visibility Checkboxes** | Hides/Shows the tool's helper actors for a clean final look. |

---

## 📦 Installation

1.  Download the repository and extract the files.
2.  Copy the `SunPointer` folder into your project's `Plugins` directory.
3.  Restart Unreal Engine.
4.  Enable **Show Plugin Content** in your Content Browser settings to locate the widget.

---

## 🤝 Contributing
Sun Pointer was built to streamline the environment art workflow. If you have ideas for improvements, new features, or find a bug, please open an issue or submit a pull request!
