# Learning of gits    -- by SC

## notes
1. 查看git版本

 ```
 git -v//查看git版本
 ```

2. 初始化仓库

 ```
 git init
 ```

3. 添加文件

 ```
 git add filename.
 ```

4. 所提交信息

 ```
 git commit -m "msg"
 ```

5. 查看状态 & 从缓存区移除文件

 ``` 
 git status
 ```

 ```
 git rm --cached file 
 ```

6. 第一次创建远程repos

 ```
 git remote add origin git@github.com:usr/name.git
 ```

7. 将缓存区内容推入repos

 ```
 git push -u origin main
 ```