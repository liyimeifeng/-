
========����ѹdemo.apk����ѹdex2jarѹ����
========���ҵ�demo.zip�е�classes.dex�ļ���������dex2jar��ѹ��Ŀ¼��cmd����ͬ����Ŀ¼
          ִ�� d2j-dex2jar classes.dex
	  û������ת���ɹ���classes-dex2jar.jar��������ת��������jar�ļ�
========��ʹ��jd-gui���ߴ�classes.dex2jar.jar�ļ�


========��������ԭʼ��Դ�ļ�,��ѹapktoolѹ������ʹ�����°��apktool.jar
========����demo.apk������apktool.jar����Ŀ¼��cmd�����Ŀ¼
	  ִ�� apktool d demo.ap
          �������쳣���ɹ����������exception��������ʹ�ù��ϰ汾apktool���з��������
          ��C:\Users\Administrator\apktool\framework���Ŀ¼������һ������Ϊ1.apk�Ļ����ļ���
	  ����������ļ�ɾ������Ȼ��������ִ�з���������


========�����´��������apktool�������İ�Ŀ¼��cmdִ��
          apktool b demo -o new_demo.apk  (b��ʾbuild��-oָ�������ɵ�apk�ļ���)
	  ʹ��AS����һ���򵥵�ǩ���ļ������µ�apk����ǩ��
          jarsigner -verbose -sigalg SHA1withRSA -digestalg SHA1 -keystore ǩ���ļ��� -storepass ǩ������ ��ǩ����APK�ļ��� ǩ���ı���

