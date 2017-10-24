import re
line='''我的电子邮件tom@gmail.com.发送到jerry123@163.com或者3123432@qq.com.
若遇到特殊情况打电话给182123445678.'''
a=re.search(r'[\w-]+(\.[\w-]+)*@[\w-]+(\.[\w-]+)+',line,re.A)
print('邮箱一：', a)
b=re.search(r'[\w-]+(\.[\w-]+)*@?163.com',line,re,A)
print('邮箱二：'，b)
c=re.search(r'[\w-]+(\.[\w-]+)*@?qq.com',line,re,A)
print('邮箱二：'，c)
d=re.search(r'(\d+){12}',line)
print('电话号码:',d)
