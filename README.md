# meiduo_project
美多商城项目，学习研究django使用

1.虚拟环境统一管理
    linux环境：
    1.安装virtualenvwrapper
        pip install virtualenv
        pip install virtualenvwrapper
    2.设置环境变量
        export WORKON_HOME=~/Envs
    3.创建虚拟环境管理目录
        mkdir -p $WORKON_HOME
    4.在~/.bashrc文件里配置环境变量，添加下面两行
        vim ~/.bashrc
        export WORKON_HOME=~/Envs
        source /usr/bin/virtualenvwrapper.sh
    5.重新加载使环境变量生效
        source ~/.bashrc
    
    windows环境
        pip install virtualenv
        pip install virtualenvwrapper-win
        设置系统环境变量 WORKON_HOME= '设置你想统一管理虚拟环境的路径'
        创建虚拟环境 mkvirtualenv test ( 此环境在你刚才配置的环境变量路径下)
        创建指定python版本的虚拟环境 mkvirtualenv -p python3 test
        查看所有虚拟环境 workon
        进入虚拟环境 workon xxx
        退出虚拟环境 deactivate
        删除虚拟环境 mvirtualenv test(虚拟环境名称)
        查看虚拟环境下的安装包 pip list
        
    生成项目所需要的的第三方包依赖文件
    pip freeze >requirements.txt
    安装
    pip install -r requirements.txt
        