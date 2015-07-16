# Dissertation

运行DIMACS提供的标准化代码时，出现了getline变量报错，原因是linux系统内置的getline和代码中的冲突,用以下代码可以解决问题：
sed -i 's/getline/apache_getline/' Instance.c
引用网页：http://www.cambus.net/compiling-apache-1.3.x-on-modern-linux-distributions/

test data list:
./portgen 1000 1000 > E1k.0
./portgen 1000 10001 > E1k.1
./portgen 1000 10002 > E1k.2
./portgen 1000 10003 > E1k.3
./portgen 1000 10004 > E1k.4
./portgen 1000 10005 > E1k.5
./portgen 1000 10006 > E1k.6
./portgen 1000 10007 > E1k.7
./portgen 1000 10008 > E1k.8
./portgen 1000 10009 > E1k.9
./portgen 3162 3162 > E3k.0
./portgen 3162 31621 > E3k.1
./portgen 3162 31622 > E3k.2
./portgen 3162 31623 > E3k.3
./portgen 3162 31624 > E3k.4
./portgen 10000 10000 > E10k.0
./portgen 10000 100001 > E10k.1
./portgen 10000 100002 > E10k.2
./portgen 31623 31623 > E31k.0
./portgen 31623 316231 > E31k.1
./portgen 100000 100000 > E100k.0
./portgen 100000 1000001 > E100k.1
./portgen 316228 316228 > E316k.0
./portgen 1000000 1000000 > E1M.0
./portgen 3162278 3162278 > E3M.0
./portgen 10000000 10000000 > E10M.0
