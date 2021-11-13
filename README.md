# Tricks on Motion Capture and Machine Learning
本仓库旨在积累一些项目开发中的经验，尤其是针对无法很好用语言描述的或网上说法不一的问题，在实际验证后在此记录其中的一些细节。

 - 查看：由于目前内容不多，暂时都以超链接的形式放在README文档，之后会进一步整理，使整体内容结构更加清晰。
 - 添加：可以通过pull request的方式添加条目，然后由项目管理者审核通过。
 - 追溯：每份文档都要求添加作者，以便他人有不懂时可以联系


## **环境配置**

 - [Windows和Ubuntu双系统安装](https://github.com/stevenzolo/Mocap_Learning_Tricks/blob/main/%E7%8E%AF%E5%A2%83%E9%85%8D%E7%BD%AE/%E5%9C%A8Windows%E4%B8%8A%E5%AE%89%E8%A3%85Ubuntu%E5%8F%8C%E7%B3%BB%E7%BB%9F.md)
 - [创建Python虚拟环境](https://github.com/stevenzolo/Mocap_Learning_Tricks/blob/main/%E7%8E%AF%E5%A2%83%E9%85%8D%E7%BD%AE/Python%E5%88%9B%E5%BB%BA%E8%99%9A%E6%8B%9F%E7%8E%AF%E5%A2%83.md)
 - [TensorFlow-gpu安装思路](https://github.com/stevenzolo/Mocap_Learning_Tricks/blob/main/%E7%8E%AF%E5%A2%83%E9%85%8D%E7%BD%AE/tensroflow-gpu%E5%AE%89%E8%A3%85%E6%80%9D%E8%B7%AF.md)
 - [DeepMimic实现过程记录](https://github.com/stevenzolo/Mocap_Learning_Tricks/blob/main/%E7%8E%AF%E5%A2%83%E9%85%8D%E7%BD%AE/DeepMimicImplement.docx)

## 搭建机器学习代码

 - 使用Python编写代码时，一致的书写风格能够提高合作效率：[Python 风格指南 - 内容目录](https://zh-google-styleguide.readthedocs.io/en/latest/google-python-styleguide/contents/)
 - [Paperwithcode](https://paperswithcode.com/) 网站提供了很多机器学习论文及其中的代码实现仓库，并且对标准问题有效果比较（Benchmark）
 - 一种自动化进行超参数调整的工具：[Optuna](https://optuna.org/)，在给定的范围内，进行有限次的尝试。和Tensorboard搭配可以一边调参一边查看效果，然后根据可视化的训练过程来选择对应的超参数组合。Optuna还能提前结束明显劣质的训练，节约时间。

### 强化学习（RL）
强化学习包括智能体和环境两部分，粗略地说，可以将环境视为待求解的问题模型，智能体是强化学习算法。

 - RL环境集成平台：[OpenAI Gym](https://gym.openai.com/)，里面提供了包括经典控制、Atari游戏、Mujoco仿真机器人等环境，基本覆盖了强化学习的常见场景。
 - RL算法集成平台，主要是深度强化学习算法：
	 - [Stable baseline](https://stable-baselines3.readthedocs.io/en/master/)：代码的[TensorFlow版](https://github.com/hill-a/stable-baselines)，[Pytorch版](https://github.com/DLR-RM/stable-baselines3)
	 - [rllab](https://rllab.readthedocs.io/en/latest/)
 - 多智能体强化学习环境集成平台：[Petting Zoo](https://www.pettingzoo.ml/)
 - 中文社区（微信公众号同名），[深度强化学习实验室](http://deeprl.neurondance.com/)

### 深度学习
TO do later!
## 动作捕捉的笔记

 - [四元数计算笔记](https://github.com/stevenzolo/Mocap_Learning_Tricks/blob/main/%E5%8A%A8%E6%8D%95%E7%AC%94%E8%AE%B0/Quaternion_calculation_notes.pdf)
 - [相邻肢体运动链的运动学计算](https://github.com/stevenzolo/Mocap_Learning_Tricks/blob/main/%E5%8A%A8%E6%8D%95%E7%AC%94%E8%AE%B0/Two-segment_chain_kinematics_tutorial.pdf)
 - 早期的[动捕介绍PPT](https://github.com/stevenzolo/Mocap_Learning_Tricks/blob/main/%E5%8A%A8%E6%8D%95%E7%AC%94%E8%AE%B0/Mocap_Intro.pptx)和[人体动捕算法综述](https://github.com/stevenzolo/Mocap_Learning_Tricks/blob/main/%E5%8A%A8%E6%8D%95%E7%AC%94%E8%AE%B0/%E4%BA%BA%E4%BD%93%E5%8A%A8%E6%8D%95%E7%AE%97%E6%B3%95%E7%BB%BC%E8%BF%B0.docx)
 - 一些可能用到的网站：
	 - 荷兰惯性动捕企业[Xsens的技术研究](https://www.xsens.com/research?document=All%20documents)
	 - [国际生物力学学会](https://isbweb.org/)提供了人体骨骼、肌肉等结构的名称和一般运动机理
	 - 斯坦福大学的人体运动康复仿真平台[OpenSim](https://opensim.stanford.edu/)
	 - 四元数、轴角、欧拉角的[在线转换网站](https://www.andre-gaschler.com/rotationconverter/)
	 - 四元数/欧拉角的转换及可视化[网站](https://quaternions.online/)

