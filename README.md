# HRmanager
用java+sqlserver做的一个人事管理系统


1、需要的环境：windows系统、jdk
2、需要的开发工具：eclipse、sql sever的DBMS
3、在eclipse中导入程序项目：
打开菜单file->import->general->existing project into space.在select root directory中选中要打开的文件夹即可。此时如果选择copy existing project into workspace就会同时将文件拷贝到workspace下。这里首先要保证要保证Eclipse两个文件.classpath和.project还在，不然无法导入，就是说Eclipse的import只认自己家的东西。
4、在DBMS中导入数据库文件：  
  选择新建查询执行下列命令：
          EXEC sp_attach_db @dbname= 'HRManager',
         @filename1 = 'mdf文件路径.MDF',
         @filename2 = 'ldf文件路径.LDF'
5、可能出现的问题：
	一、打开的工程与Eclipse的配置不同，在运行时会产生问题。解决方法是：
打开菜单project->properties修改。主要需要修改的是java build path项。
可参考：https://blog.csdn.net/Axela30W/article/details/76255226
	二、没有成功连接数据库，解决方法是：
参考：https://blog.csdn.net/qinyf2015/article/details/54378070
	
