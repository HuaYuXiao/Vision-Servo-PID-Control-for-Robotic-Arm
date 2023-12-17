# Vision Servo PID Control for Robotic Arm

![HitCount](https://img.shields.io/endpoint?url=https%3A%2F%2Fhits.dwyl.com%2FHuaYuXiao%2FAdaptive-Vision-Servo-for-Robotic-Arm-Automatic-Gripping-System.json%3Fcolor%3Dpink)
![Static Badge](https://img.shields.io/badge/ROS-kinetic-22314E?logo=ros)
![Static Badge](https://img.shields.io/badge/Ubuntu-16.04-E95420?logo=ubuntu)
![Static Badge](https://img.shields.io/badge/Python-_-3776AB?logo=python)
![Static Badge](https://img.shields.io/badge/TensorFlow-_-FF6F00?logo=tensorflow)
![Static Badge](https://img.shields.io/badge/OpenAI-_-412991?logo=openai)
![Static Badge](https://img.shields.io/badge/Google_Translate-_-4285F4?logo=googletranslate)

On the KINOVA Gen3 lite robotic arm, an adaptive visual servoing automatic grasping system is implemented. After obtaining the grasping target from natural language instructions, the precise positioning of the target object is achieved with the help of MediaPipe, and the grasping angle and path are designed and generated by ourselves. Using a self-developed adaptive visual servoing algorithm, the object is grasped to a specified position.

## 如何运行

Download all files under the `code` folder, and then run the `main.py` file.

Note: Before running, make sure to modify the reference files to the appropriate location on your computer.

![image](https://github.com/HuaYuXiao/Visual-servo-NLP-based-6DOF-Manipulator-Grasp-System/assets/100033111/668a3de3-0216-46da-9722-6250f476714b)

## 历史版本

### 2023年9月3日

新增了以下内容：首先通过实时语音输入或文字输入，然后基于[OpenAI](https://github.com/chatanywhere/GPT_API_free)与Google翻译两个接口，实现NLP语义理解，最后输出目标物品的名字。

具体代码详见[NLP](https://github.com/HuaYuXiao/Visual-servo-NLP-based-6DOF-Manipulator-Grasp-System/tree/main/code/NLP)文件夹下的两个程序。

```bash
D:\software\anaconda3\python.exe D:\iCloudDrive\项目\NLP\代码\main.py 
请告诉我你的需求：我喜欢冰箱和苹果，我讨厌山和香蕉，他超爱梨和鸭子。
喜欢的物品：冰箱、苹果、梨、鸭子。
['refrigerator', 'apple', 'pear', 'Duck']

Process finished with exit code 0
```

## Contributions
- Hongjing Tang: visual-servo control and camera configuration
- Yuxiao Hua: multi-thread, NLP and final report
- Xizhe Hao: voice control and PPT presentation
  
