在后续的文章中，将不再区分linux环境还是windows环境。因为linux环境和windows环境的区别只是生成.img的方式不同，但最终的目的都是生成.img文件。
linux下自己写.ld文件和makefile文件，把源码编译链接成可执行文件，最后通过dd生成.img。
windows下使用nasm把汇编源码编译链接成可执行文件，通过WinImage或UE生成.img。
生成后的.img只要符合标准，可以在任何虚拟机上跑，比如bochs、virtualbox。只不过不同的虚拟机个有优缺点，在于自己的取舍。并不是一定要按照前文中所给的方法，在windows上一定要用bochs或在linux上一定要用virtualbox。

《运行自己的操作系统》系列后续的文章都是基于以下方式开发的：

||||
|---|---|---|---|
|编译|	linux系统|	g++|
|链接|	linux系统|	ld|
|生成镜像文件	linux系统	dd|
|调试|	windows系统|	bochs|
|运行|	windows系统|	virtualbox|

参加文献：
《write-os-weekly》
《30天自制操作系统》
《linux内核完全剖析》   