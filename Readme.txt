
========》解压demo.apk，重命名为demo.zip,解压缩，然后解压dex2jar压缩包
========》找到demo.zip中的classes.dex文件，拷贝到dex2jar解压后目录，cmd进入同样的目录
          执行 d2j-dex2jar classes.dex
	  没报错，即转换成功，classes-dex2jar.jar就是我们转换出来的jar文件
========》使用jd-gui工具打开classes.dex2jar.jar文件


========》反编译原始资源文件,解压apktool压缩包，使用最新版的apktool.jar
========》将demo.apk拷贝到apktool.jar所在目录，cmd进入该目录
	  执行 apktool d demo.ap
          不出现异常即成功，如果出现exception，可能是使用过老版本apktool进行反编译过，
          将C:\Users\Administrator\apktool\framework这个目录下生成一个名字为1.apk的缓存文件，
	  将这个缓存文件删除掉，然后再重新执行反编译命令


========》重新打包，进入apktool反编译后的包目录，cmd执行
          apktool b demo -o new_demo.apk  (b表示build，-o指定新生成的apk文件名)
	  使用AS生成一个简单的签名文件，对新的apk进行签名
          jarsigner -verbose -sigalg SHA1withRSA -digestalg SHA1 -keystore 签名文件名 -storepass 签名密码 待签名的APK文件名 签名的别名

