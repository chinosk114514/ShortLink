# ShortLink
 - ʹ��Flask+MySQL���в������������

# ����:
 - ��Ҫ`Python3`�����Լ�`Flask`,`pymysql`ģ��  
 - ��Ҫһ��������MySQL����,����׸��  
 - ����һ�����ݿ������`shortlink.sql`��ʼ��һ�ű�  
 - ��д`connect_settings.py`���������  
 - ����
 
# ���/ɾ������(�ֶ�)
 - ���:�ο�`add_link_example.bat`  
 - ɾ��:�ֶ�ɾ���ݿ��  
 (���������API��ӷ�ʽ)
  
# ���/ɾ������(API)
����
```
http://��������/api?����
```
|����|����|����|��ע|
|:-:|:-:|:-:|:-:|
|key|������Կ|Yes|����`connect_settings.py`�����õ�key|
|type|������ʽ|Yes|������д`add`��`del`|
|link|�����������|Yes|`type`Ϊ`add`ʱ,������ַ<br>`type`Ϊ`del`ʱ,��������Ӻ�׺��������������|
|creator|���Ӵ�����|No|��¼������<br>����`type`Ϊ`add`ʱ��Ч|
|from|���Ӵ�������Դ|No|��¼��������Դ(Ⱥ��,��վ��)<br>����`type`Ϊ`add`ʱ��Ч|

���õ������������
```
http://127.0.0.1:5000/api?key=QnuGfefJIhuGYUF84&type=del&link=sicr
http://127.0.0.1:5000/api?key=QnuGfefJIhuGYUF84&type=del&link=http://myweb.site/sicr
http://127.0.0.1:5000/api?key=QnuGfefJIhuGYUF84&type=add&link=http://www.baidu.com&creator=123&from=qwq
```