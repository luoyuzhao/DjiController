# DjiController 2.0

因部分原因，暂不开源3D版本，本版本为2D基础版本，仅供参考，该飞行策略会导致续航时间缩短，有待优化


3D版本请参照https://github.com/luoyuzhao/amap3dDrawingExtension 自行扩展。

#contact-email:290330505@qq.com

！！本软件不保证飞行安全，使用所产生一切后果自行承担！！

！！本软件不保证飞行安全，使用所产生一切后果自行承担！！

根据大疆SDK定制航飞客户端
特性：


/*基于高德地图叠加谷歌卫星图层

/*KML范围线导入查看

/*绘制航飞区域

/*大范围任务（航点超过99，航线超过3公里）

/*测距离侧面积

/*根据相机参数和重叠度自动计算航高(也可手动指定飞行高度或返航高度)

/*测区局部增加变高区域（飞入时按此区域高度飞行，飞出时恢复测区原本高度）

/*任务状态持久化

/*根据飞机实时位置自行实现状态更新，不依赖大疆内部触发器（实测在丢失信号至信号恢复后，触发器会失效）

/*修正当丢失信号一段时间以后，再次连接时，偶尔会触发强制返航的问题

安全策略：
飞行默认日本手，不开启蔽障模式，当信号丢失会继续执行飞行任务不返航
直至电量只够返航时将会强制返航，下一次继续执行可手动选择起始位置。 
当电量低于35%触发报警，低于20%会强制返航
无半径限制和航线范围限制

![界面UI1](https://github.com/luoyuzhao/DjiController/blob/master/Screenshot_01.png)

![界面UI2](https://github.com/luoyuzhao/DjiController/blob/master/Screenshot_02.png)
