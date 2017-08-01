# Jbox2dProject
## 思路
1. 创建一个JboxImpl类，专门用于管理刚体和世界的创建和逻辑计算
2. 自定义一个view，这里为了方便直接继承FrameLayout，并且在真实屏幕中将JboxImpl中计算出刚体运动的坐标绑定给真实的view（也就是这里的image），根据重力感应不停的回调绘制。
3. MainActivity中做重力感应的注册，回调的变化传递到jboxView进行界面重绘。
