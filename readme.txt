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
Ҫ�鿴Զ�̿����Ϣ����git remote��

$ git remote
origin
���ߣ���git remote -v��ʾ����ϸ����Ϣ��

$ git remote -v
origin  git@github.com:michaelliao/learngit.git (fetch)
origin  git@github.com:michaelliao/learngit.git (push)
������ʾ�˿���ץȡ�����͵�origin�ĵ�ַ�����û������Ȩ�ޣ��Ϳ�����push�ĵ�ַ��

���ͷ�֧
���ͷ�֧�����ǰѸ÷�֧�ϵ����б����ύ���͵�Զ�̿⡣����ʱ��Ҫָ�����ط�֧��������Git�ͻ�Ѹ÷�֧���͵�Զ�̿��Ӧ��Զ�̷�֧�ϣ�

$ git push origin master
���Ҫ����������֧������dev���͸ĳɣ�

$ git push origin dev
���ǣ�������һ��Ҫ�ѱ��ط�֧��Զ�����ͣ���ô����Щ��֧��Ҫ���ͣ���Щ����Ҫ�أ�

master��֧������֧�����Ҫʱ����Զ��ͬ����

dev��֧�ǿ�����֧���Ŷ����г�Ա����Ҫ�����湤��������Ҳ��Ҫ��Զ��ͬ����

bug��ֻ֧�����ڱ����޸�bug����û��Ҫ�Ƶ�Զ���ˣ������ϰ�Ҫ������ÿ�ܵ����޸��˼���bug��

feature��֧�Ƿ��Ƶ�Զ�̣�ȡ�������Ƿ�����С�����������濪��
=============================================================================
git add -A�� git add .   git add -u�ڹ����Ͽ��ƺ�����������Ǵ���һ����

git add . �������ع�������״̬����ʹ������ѹ���ʱ�����б仯�ύ���ݴ����������ļ������޸�(modified)�Լ����ļ�(new)������������ɾ�����ļ���

git add -u ����������Ѿ���add���ļ�����tracked file�������Ὣ���޸ĵ��ļ��ύ���ݴ�����add -u �����ύ���ļ���untracked file������git add --update����д��

git add -A ���������������ܵĺϼ���git add --all����д��
======================================================================
����ʧ�ܣ���Ϊ���С���������ύ������ͼ���͵��ύ�г�ͻ������취Ҳ�ܼ򵥣�Git�Ѿ���ʾ���ǣ�����git pull�����µ��ύ��origin/devץ������Ȼ���ڱ��غϲ��������ͻ�������ͣ�

$ git pull
There is no tracking information for the current branch.
Please specify which branch you want to merge with.
See git-pull(1) for details.

    git pull <remote> <branch>

If you wish to set tracking information for this branch you can do so with:

    git branch --set-upstream-to=origin/<branch> dev
git pullҲʧ���ˣ�ԭ����û��ָ������dev��֧��Զ��origin/dev��֧�����ӣ�������ʾ������dev��origin/dev�����ӣ�

$ git branch --set-upstream-to=origin/dev dev
Branch 'dev' set up to track remote branch 'dev' from 'origin'.
��pull��

$ git pull
Auto-merging env.txt
CONFLICT (add/add): Merge conflict in env.txt
Automatic merge failed; fix conflicts and then commit the result.
���git pull�ɹ������Ǻϲ��г�ͻ����Ҫ�ֶ����������ķ����ͷ�֧�����еĽ����ͻ��ȫһ����������ύ����push��
==============================================================
��ˣ�����Э���Ĺ���ģʽͨ����������

���ȣ�������ͼ��git push origin <branch-name>�����Լ����޸ģ�

�������ʧ�ܣ�����ΪԶ�̷�֧����ı��ظ��£���Ҫ����git pull��ͼ�ϲ���

����ϲ��г�ͻ��������ͻ�����ڱ����ύ��

û�г�ͻ���߽������ͻ������git push origin <branch-name>���;��ܳɹ���

���git pull��ʾno tracking information����˵�����ط�֧��Զ�̷�֧�����ӹ�ϵû�д�����������git branch --set-upstream-to <branch-name> origin/<branch-name>��

����Ƕ���Э���Ĺ���ģʽ��һ����Ϥ�ˣ��ͷǳ��򵥡�

С��
�鿴Զ�̿���Ϣ��ʹ��git remote -v��

�����½��ķ�֧��������͵�Զ�̣��������˾��ǲ��ɼ��ģ�

�ӱ������ͷ�֧��ʹ��git push origin branch-name���������ʧ�ܣ�����git pullץȡԶ�̵����ύ��

�ڱ��ش�����Զ�̷�֧��Ӧ�ķ�֧��ʹ��git checkout -b branch-name origin/branch-name�����غ�Զ�̷�֧���������һ�£�

�������ط�֧��Զ�̷�֧�Ĺ�����ʹ��git branch --set-upstream branch-name origin/branch-name��

��Զ��ץȡ��֧��ʹ��git pull������г�ͻ��Ҫ�ȴ����ͻ��
