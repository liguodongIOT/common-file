## ���

oozie������hadoopƽ̨�Ŀ�Դ��������������
��������hadoop��ҵ
����webӦ�ó�����oozie client��oozie server����������ɡ�
oozie server������Java servlet������Tomcat���е�web����



## �� ��

ͳһ����hadoopϵͳ�г�����MR����������hdfs������shell���ȣ�hive������
�ǵĸ��Ƶ�������ϵ��ʱ�䴥����ʱ�䴥��ʹ��xml���Խ��б�����Ч����ߡ�
һ������ʹ��DAG����ʾ��ʹ��ͼ�α���߼���������
֧�ֺܶ���������ȣ�����ɴ󲿷�hadoop������
������֧��EL�����ͺ����������ḻ��

web�����ַ
http:oozie.host.ip:11000/oozie/

## oozie����

�����б�鿴
����״̬�鿴
���̷�����Ϣ
�ڵ���Ϣ�鿴
����ͼ��Ϣ
��־�鿴
ϵͳ��Ϣ�鿴������



## oozie cli ���

��������
oozie job -oozie http://ip:11000/ -config job.properties -run


ֹͣ����
oozie job -oozie http://ip:11000/ -kill 0032-dsda-434343-43fs(����ID)


�ύ����
oozie job -oozie http://ip:11000/ -config job.properties -submit


��ʼ����
oozie job -oozie http://ip:11000/ -config job.properties -start 0032-dsda-434343-43fs



��������
oozie job -oozie http://ip:11000/ -config job.properties -info 0032-dsda-434343-43fs



## JOB ���� job.properties



## �ڵ�

A.���̿��ƽڵ�
start-����workflow��ʼ
end-����workflow����
decision-ʵ��switch����
sub-workflow-������workflow
kill-ɱ��workflow
fork-����ִ��workflow
join-����ִ�н�������forkһ��ʹ�ã�


B.�����ڵ�
shell
java
fs
MR
hive
sqoop



shell�ڵ�

--job.properties



--workflow.xml





impala --�����Ż�

�� -- �ڴ桢C++ ������MR��ʽ��data local

��ʽ�洢�����ݲֿ�



impala VS hive��ϵ

ȱ�㣺�ڴ桢����̫�����������ģ�hive����̫��



�ܹ� 

catalog statestore        (impalad ����Э��)



shell -p  explain profile

 -r  refresh

-f -o -i



impala sql ��hive sql

��������  �������Ͳ�֧��

һЩ������֧��



impala���ݴ���






























