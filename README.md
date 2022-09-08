##
    www.liaoxuefeng.com

## 安装
    官网下载默认配置

## 初始化身份
    git config --global user.name "Your Name"
    git config --global user.email "email@example.com"

## 创建仓库
    初始化仓库： git init

## 添加到仓库
    git add filename

## 提交到仓库
    git commit -m '注释'    // 注释一定要写，比如'增加了一个文件'

## 时光穿梭
    git status:查看仓库状态  看仓库里有没有未提交的
    git diff  :查看仓库状态  查看具体改变内容
    git log   :查看历史版本
    git log --pretty=oneline  :查看历史版本(简洁版) 前面的码类似于唯一id
    git reset --hard HEAD^  :回到历史版本(几个^回退几个版本)
    git reset --hard 码   :回到指定版本

## 工作区和暂存区

## 删除文件
    rm filename  :本地删除--工作区删除

    git rm filename
    git commit -m '删除文件' :版本库删除

    git checkout -- filename :找回文件(工作区删除，版本库未删除)

## 分支管理
    创建并切换分支： git checkout -b <name>     
        git checkout  代表创建分支
        -b     代表切换分支
        dev    代表分支名称
        创建一个叫<name>的分支并切换过去

    查看分支 git branch
    创建分支 git branch <name>
    切换分支 git checkout <name>
    合并某分支到当前分支  git merge <name>
    删除分支 git branch -d <name>

## 推送到远程仓库
    github平台
        1.生成ssh
            ssh-keygen -t rsa -C "1010292707@qq.com"
        2.关联github
        3.创建仓库
        4.把本地仓库代码推送到远程仓库

    gitee平台
        1.克隆仓库：
            git clone https://gitee.com/cher1sh0312/test.git
        2.上传操作
        3.多人协作

    远程仓库的命令
        git clone url
        git push
        git pull