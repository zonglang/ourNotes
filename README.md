# 一个小小小说明

> 一般合作开发是fork一个项目，然后提mergeRequest合并提交
>
> 但是我们这个小团体就不这么麻烦了，直接每个人都加collaborators权限

### 如何在本地跑起gitbook

1. 需要全局安装gitbook-cli

   ```
   npm install -g gitbook-cli 
   ```

2. 克隆项目到本地

   ```
   git clone git@github.com:zonglang/ourNotes.git
   ```

3. 进入项目目录

   ```
   cd ourNotes/
   ```

4. ~~项目初始化，安装插件什么的~~(已将node_modules上传到仓库，不需要这一步了)

   ```
   gitbook install 
   ```

4. 本地起一个服务

   ```
   gitbook serve
   ```

5. 然后就可以访问本地的4000端口

### gitbook构建原则

面试的点和面都很宽泛，所以我们需要一个系统化的面试解决方案。

在面试之前有一个提纲，就成为了刚需。

目前我们的使用原则是：

1. 在issue上提出零碎的点，然后大家把自己的对知识点的理解，或者看到的好的文章贴上去。
2. 本地clone一个gitbook，用作自己的笔记。
3. 一个知识点的issue足够完善之后，我们汇总到gitbook远程仓库中

### 如何协作

我们只维护一个主分支master，所以为了使版本管理有序，请在push之前进行以下[变基操作](https://git-scm.com/book/zh/v2/Git-%E5%88%86%E6%94%AF-%E5%8F%98%E5%9F%BA)

```
git pull --rebase
```

