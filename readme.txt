Git help
��������ֻҪ���������ύ���Ϳ���ͨ�����
git push origin master

���ڣ����Ǹ���GitHub����ʾ���ڱ��ص�learngit�ֿ����������

$ git remote add origin git@github.com:michaelliao/learngit.git

�Ϳ��԰ѱ��ؿ�������������͵�Զ�̿��ϣ�

$ git push -u origin master
=====================================================-----------
Ҫ����һ��Զ�̿⣬ʹ������git remote add origin git@server-name:path/repo-name.git��

������ʹ������git push -u origin master��һ������master��֧���������ݣ�

�˺�ÿ�α����ύ��ֻҪ�б�Ҫ���Ϳ���ʹ������git push origin master���������޸ģ�
С��
Git��������ʹ�÷�֧��

�鿴��֧��git branch
���ȣ����Ǵ���dev��֧��Ȼ���л���dev��֧��

$ git checkout -b dev
===============================================================


������֧��git branch <name>

�л���֧��git checkout <name>����git switch <name>

����+�л���֧��git checkout -b <name>����git switch -c <name>

�ϲ�ĳ��֧����ǰ��֧��git merge <name>

ɾ����֧��git branch -d <name>
===============================================================


׼���ϲ�dev��֧����ע��--no-ff��������ʾ����Fast forward��

$ git merge --no-ff -m "merge with no-ff" dev

===============================================================

