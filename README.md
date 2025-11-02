# Kortex-gen3-lite-robot-arm Description

This repository contains the **URDF** files  for visualizing and simulating the Kortex-gen3-lite robot arm in  **RViz2**.
---

## Requirements
- **Ros2 Humble or other versions**
- **urdf_tutorial** package
- **RViz2**
## Expected Result
<img width="1416" height="921" alt="image" src="https://github.com/user-attachments/assets/a07f8f29-222c-47be-aed7-6e3e3fb67518" />


## How to use the repo

### 1. Create a workspace- a folder e.g
```bash
mkdir kortex-gen3-ws
```

### 2. Clone the Repo

Navigate to your workspace
```bash
cd kortex-gen3-ws
```

Clone this repository into your workspace:

```bash
git clone https://github.com/LANRAY01/kortex-gen3-lite-robot-arm

```

### 3. Check for Dependencies

Verify that your workspace detects the package:

```bash
colcon list
```

If dependencies are missing, make sure to install them before proceeding.

### 4. Build the Package

```bash
colcon build
```

### 5. Source the Setup File

After building, source your workspace environment:

```bash
source install/setup.bash
```
### 6. Run the package
```bash
ros2 launch urdf_tutorial display.launch.py model:=/$PWD/kortex-gen3_lite_description/urdf/arm.urdf
```





