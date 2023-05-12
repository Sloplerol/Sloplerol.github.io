# Satrol_的个人网站

[https://sloplerol.github.io/](https://sloplerol.github.io/)

* theme:[Butterfly](https://github.com/jerryc127/hexo-theme-butterfly)

* Bufferfly disposition: [deposition](https://butterfly.js.org/posts/4aa8abbe/#%E7%B6%B2%E7%AB%99%E8%B3%87%E6%96%99)

* How to Build with hexo



# Install Homebrew

参考CSDN:[https://blog.csdn.net/qq_43783527/article/details/125242300](https://blog.csdn.net/qq_43783527/article/details/125242300)






# Install Nodejs

```
brew install node
```

`node -v查询是否安装成功`





# Basic Operation

* 创建一个文件夹

    ```
    mkdir 文件名
    ```

* 初始化文件夹

    ```
    hexo init
    ```

* 本地启动服务

    ```
    hexo s
    ```

* 在当前文件内部的_posts文件中新建一个md文档,写入内容



# Github Page 运用

* 新建一个仓库起名为你的用户名.github.io

* 回到cd到博客文件的终端，安装git部署插件

    ```
    npm install hexo-deployer-git --save 
    ```

* 更改blog文件夹下的_config.yml文件，在文件最下方添加如下内容，repo为新建的仓库地址

    ```
    # Deployment
    ## Docs: https://hexo.io/docs/one-command-deployment
    deploy:
      type: git
      repo: 你的仓库地址 ssh和http两种地址都行
      branch: master
    
    ```

* 依次执行以下操作

    ```
    //清理缓存
    hexo clean
    //生成
    hexo g
    //启动服务(他会提醒你在本地的那个端口可以预览)
    hexo s 
    ```

* 部署(相当于帮你上传文件到你个人博客的仓库中)

    ```
    hexo d
    ```

* 检验是否部署成功

    ```
    查看个人博客仓库Action中是否打绿勾
    ```

    





