# Dissertation

运行DIMACS提供的标准化代码时，出现了getline变量报错，原因是linux系统内置的getline和代码中的冲突,用以下代码可以解决问题：
sed -i 's/getline/apache_getline/' Instance.c
引用网页：http://www.cambus.net/compiling-apache-1.3.x-on-modern-linux-distributions/
