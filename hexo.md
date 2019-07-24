# hexo 博客安装以及next主题安装
`git clone -b hexo git@github.com:883901/883901.github.io.gi`

`npm install hexo --save`

`git add . `  添加所有文件到暂存区

`git commit -m ""` 提交，""里面填更新的标题

`git push origin hexo` 推送hexo分支到github

注意，以上所有的步骤都已经执行过本地关联远程仓库操作了。

`git remote add origin git@github.com:883901/883901.github.io.git`

## 安装hexo配置next主题

`npm install -g hexo-cli`
## 到hexo文件夹、部署hexo文件、安装依赖
```
cd /d/hexo
hexo init
npm install
```
_config.yml  为网站的 配置 信息
## 安装主题
`git clone https://github.com/theme-next/hexo-theme-next themes/next`
修改网站配置文件主题为：next
## 配置github链接文件设置
```
deploy:
  type: git
  repository: git@github.com:883901/883901.github.io.git
  branch: master
```
可把备份的文章直接放到 _posts文件夹呢
修改主题配置文件，参考[https://theme-next.org/docs/getting-started/](https://theme-next.org/docs/getting-started/)

注：```npm install --save hexo-deployer-git```   （上床到github失败时）
