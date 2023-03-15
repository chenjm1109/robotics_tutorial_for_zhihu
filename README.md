# 开源机器人学

机器人爱好者您好，这是一个帮助机器人学习者入门的开源项目，包含以下内容：

- 机器人学基础知识点与算法的Python实现
- 可用于指导学习的机器人建模工具箱
- 可用于验证机器人学算法正确性的**测试用例**与**实验数据**

本项目是作者根据多年学习和工作经验总结出来的，具有以下特点：

- 贴合实际工程经验与使用习惯
- 核心计算完全采用 Modern Robotics 旋量代数方法
- 充分注释，重视可读性

本项目将持续更新，感谢您的关注~

## 快速使用

## 打包安装

```python
python setup.py sdist
pip install ./dist/open_robotics-1.0.0.tar
```

创建机器人实例。详细用法请查看[创建机器人的多种方法](#创建机器人的多种方法)。

```python
from open_robotics import OpenRobotics
robot = OpenRobotics('CR6')
```

查看机器人的参数

```python

```

计算正向运动学

```python
point = robot.calc_fkine([90, 45, 0, 0, 0, 0])
print(point)
```

计算逆向运动学

```python

```


## 算法说明

### 创建机器人的多种方法

### ModernRoboticsPlus

ModernRoboticsPlus(MRP) 对于 ModernRobotics 项目的改进与补充，在保证基础理论与原书一致的情况下，做了如下修改：

- 改进了一些函数的用法，使其更符合工程使用习惯：轨迹规划
- 补充了书中有所讲解、但原项目未曾实现的一些方法：轨迹规划