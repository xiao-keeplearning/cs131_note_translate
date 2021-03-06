# CS131 Lecture 1:课程介绍

## 1. 什么是计算机视觉？

### 1.1 定义

**计算机视觉有两种定义**  

计算机视觉可以被定义为一种科学领域——研究如何从数字图像中提取信息。从图像获得的信息类型会随不同的应用场景需要而变化，比如识别，导航中的空间测量或AR应用。

另外一种定义是：从应用角度来看，计算机视觉是构建能理解图像内容并将其用于其它应用的算法。我们将在第4节中看到计算机视觉在不同领域的应用。

### 1.2 跨学科领域

计算机视觉汇集了大量学科。神经科学可以通过理解人类视觉来帮助计算机视觉，我们将在第2节中看到。计算机视觉可以被视为计算机科学的一部分，算法理论以及机器学习对于开发计算机视觉算法至关重要。我们将在本课程中展示图1中的所有学科领域是如何联系在一起的，计算机视觉是如何从中吸取灵感和技术的。![fields](F:\浙大研究生\cs131\notes\cs131_notes-master\lecture01\fields.png)

### 1.3 困难的问题（略）

## 2 理解人类的视觉系统

想解决计算机视觉问题，最开始的想法是理解人的视觉是如何工作的，然后利用相关知识迁移到计算机上。

### 2.1 视觉的定义

无论是计算机还是动物，视觉系统总是可以分成两部分。

首先，传感设备从图像中捕获尽可能多的细节。眼睛将通​过虹膜捕获光线并将其投射到视网膜上，在那里有专门的细胞通过神经元将信息传递给大脑。相机以类似的方式捕获图像并将像素传输给计算机。在这一部分中，摄像机比人类表现更好，因为它们可以看到红外线，看得更远、更精确。

第二，解释装置必须处理信息并从中提取意义。人类在大脑的不同区域通过多个步骤解决了这个问题。在这一部分计算机视觉仍然落后于人类表现。

### 2.2 人的视觉系统（略）

### 2.3 为什么人类的视觉系统如此强大？

**速度** 人类视觉系统非常有效。认识到威胁并对它们作出快速反应对于生存至关重要，数百万年的进化完善了的哺乳动物视觉系统。

**人类的不足** 然而，这种速度是以一些缺点为代价获得的。改变图像的弱相关部分（例如水面反射或背景）可能会被忽视，因为人类大脑专注于图像的重要部分。如果信号非常接近背景，则可能难以检测和分割图像的相关部分。

**Context** 人们一直使用上下文来推断图像的线索。以前的知识是融入计算机视觉的最难的工具之一。人类使用上下文来知道应该关注图像哪个部分，知道在某些位置会发生什么。上下文也有助于大脑对阴影中的颜色进行补偿。但是，上下文可以用来欺骗人类的大脑。

### 2.4 来自自然的教训

模仿鸟类并没有将人类引向飞机。简单地复制自然界并不是学习如何飞行最有效的方法。但是研究鸟类让我们了解空气动力学，理解像升力这样的概念让我们能够建造飞机。

## 3 从图像中获取信息

我们可以将从图像中获得的信息分为两类：测量和语义信息。

### 3.1 视觉作为一种测量装置

在未知位置的机器人导航需要扫描周围环境以计算最佳路径。使用计算机视觉，我们可以测量机器人周围的空间并创建周边环境地图。

立体摄像机通过三角测量提供深度信息，就像我们的两只眼睛一样。立体视觉是计算机视觉领域的研究领域，并且有很多研究寻求通过给出的立体图像创建精确的深度图。

如果我们增加视角的数量以覆盖对象的所有边，我们可以创建一个对象的3D表面[2]。一个更具挑战性的想法可能是通过谷歌图像搜索这座纪念碑的所有结果来重建纪念碑的3D模型。

还有一些关于抓取的研究，其中计算机视觉可以帮助理解物体的3D几何形状，以帮助机器人抓住它。通过机器人的摄像头，我们可以识别并找到物体的手柄并推断其形状，然后使机器人找到一个良好的抓握位置。

### 3.2 语义信息的来源

除了测量信息外，图像还包含非常密集的语义信息。我们可以标记图像中的对象，标记整个场景，识别人物，识别动作，手势，人脸。

## 4 计算机视觉的应用

