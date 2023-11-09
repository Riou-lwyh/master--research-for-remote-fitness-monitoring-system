这里是Jetson端的代码。

在jetson上，运行trtpose，并将计算得到的人体骨骼点发送到server。同时，jetson端会接收来自鱼眼摄像头的模糊位置信息，并通过这个信息控制舵机旋转，指向人的方向。

trtpose的原代码来自英伟达AI-IOT的项目，项目链接如下：
https://github.com/NVIDIA-AI-IOT/trt_pose
在Jetson上配置好该项目后，按照本文件夹中的JetsonPTZ.ipynb修改live_demo.ipynb文件.
同时，原trtpose项目中的trt_pose/trt_pose文件夹中的draw_objects.py 和parse_objects.py有做一定程度的修改。
