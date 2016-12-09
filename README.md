# XcodeCleanDocument

>今天为了删除一些老旧的项目，特地查了好多资料，记下来以供以后查询


#这个就是我要找的答案，感谢starkoverflow.感谢Google
- 移除Archive过的项目 

可以删除已经归档的项目，在Organizer的列表中删除 

路径： ~/Library/Developer/Xcode/Products

- 移除对旧设备的支持 

可重新生成；再连接旧设备调试时，会重新自动生成。我移除了4.3.2, 5.0, 5.1等版本的设备支持。

路径：~/Library/Developer/Xcode/iOS DeviceSupport

- 移除旧版本的模拟器支持

不可恢复；如果需要旧版本的模拟器，就需要重新下载了。我移除了4.3.2, 5.0, 5.1等旧版本的模拟器。

路径：~/Library/Application Support/iPhone Simulator

- 移除模拟器的临时文件

可重新生成；如果需要保留较新版本的模拟器，但tmp文件夹很大。放心删吧，tmp文件夹里的内容是不重要的。在iOS Device中，存储空间不足时，tmp文件夹是可能被清空的。

路径：~/Library/Application Support/iPhone Simulator/6.1/tmp (以iOS Simulator 6.1为例)

- 移除模拟器中安装的Apps

不可恢复；对应的模拟器中安装的Apps被清空了，如果不需要就删了吧。

路径：~/Library/Application Support/iPhone Simulator/6.1/Applications (以iOS Simulator 6.1为例)

- 移除Archives

不可恢复；Adhoc或者App Store版本会被删除。建议备份dSYM文件夹

路径：~/Library/Developer/Xcode/Archives

- 移除DerivedData

可重新生成；会删除build生成的项目索引、build输出以及日志。重新打开项目时会重新生成，大的项目会耗费一些时间。

路径：~/Library/Developer/Xcode/DerivedData

- 移除旧的Docsets

不可恢复；将删除旧的Docsets文档

路径：~/Library/Developer/Shared/Documentation/DocSets
