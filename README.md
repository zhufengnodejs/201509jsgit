# 201509jsgit
2015年第九期git学习

#资料
##在线地址
http://ke.qq.com/course/103151
##课件地址
http://school.zhufengpeixun.cn/course/31
##github网址
https://github.com/
##Win8显示隐藏文件的方法
[Win8显示隐藏文件的方法](http://jingyan.baidu.com/article/066074d68ddc7cc3c21cb082.html)
##Win7显示隐藏文件的方法
[Win7显示隐藏文件的方法](http://jingyan.baidu.com/article/af9f5a2dc1f91243150a4553.html)

#安装git
> www.git-scm.com

#配置git
```
git config --global user.name "zfpx"    
git config --global user.email "zfpx@126.com" 
git config --global --list
```
#创建git仓库
```
mkdir gitstudy
cd gitstudy
git init
```

#显示隐藏目录
```
ls -al
```

#添加文件
```
echo 1 > index.html   // 把1输出到新创建的index.html文件中  > 表示清空并写入
echo 2 >> index.html // 追2加到index.html中 >>表示在原来文件的末尾追加
cat index.html //查看文件内容

git add index.html //把文件添加到暂存区
git commit index.html -m"在index.html中增加了 1 2"

git log 查看历史

```

#问题记录
1. 出现> 大于号
```git commit -m"提交文件"``
一旦输入了中文的双引号，要按`ctrl+c`退出重新执行名
2. 删除的文件
`git add` 添加的变化，不管是增加文件，还是修改文件，还是删除文件，都需要`add`

3. 文件夹下明明有**index.html**文件，`git add index.html`时却报找不到
这是因为没有显示扩展名，其实文件名是`index.html.txt`
[Win8系统中如何显示/隐藏文件扩展名](http://jingyan.baidu.com/article/48b37f8d458bc01a646488f2.html)
[win7如何显示文件后缀](http://jingyan.baidu.com/article/5d368d1e31ed903f60c057c6.html)




