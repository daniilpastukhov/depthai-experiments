[中文文档](README.zh-CN.md)

# Pose Estimation Example

This example demonstrates how to run [Human Pose Estimation Network](https://docs.openvinotoolkit.org/latest/omz_models_intel_human_pose_estimation_0001_description_human_pose_estimation_0001.html) using Gen2 Pipeline Builder.


## Demo

### Camera
[![Gen2 Age & Gender recognition](https://user-images.githubusercontent.com/5244214/107493701-35f97100-6b8e-11eb-8b13-02a7a8dbec21.gif)](https://www.youtube.com/watch?v=Py3-dHQymko "Human pose estimation on DepthAI")

### Video file

[![Gen2 Age & Gender recognition](https://user-images.githubusercontent.com/5244214/110801736-d3bf8900-827d-11eb-934b-9755978f80d9.gif)](https://www.youtube.com/watch?v=1dp2wJ_OqxI "Human pose estimation on DepthAI")

## Usage

Choose one of the following options:
```bash
# For DepthAI API
cd ./api

# For DepthAI SDK
cd ./sdk
```

### Pre-requisites

```bash
python3 -m pip install -r requirements.txt
```

### Launch the script

```bash
# For DepthAI API
python3 main.py [options]

# For DepthAI SDK
python3 main.py
```

Options:
```
usage: main.py [-h] [-nd] [-cam] [-vid VIDEO]

optional arguments:
  -h, --help            show this help message and exit
  -nd, --no-debug       Prevent debug output
  -cam, --camera        Use DepthAI 4K RGB camera for inference (conflicts with -vid)
  -vid VIDEO, --video VIDEO
                        Path to video file to be used for inference (conflicts with -cam)
```