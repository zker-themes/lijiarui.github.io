# lijiarui.github.io

Using [hexo](https://github.com/hexojs/hexo) for my blog
Using theme: [hexo-theme-jsimple](https://github.com/tangkunyin/hexo-theme-jsimple)

## DEPLOY TO GITHUB
```
hexo generate
hexo deploy
```

## FIRST RUN
Do some small change so fork to my repo: [lijiarui/hexo-theme-jsimple](https://github.com/lijiarui/hexo-theme-jsimple)
```
git clone https://github.com/lijiarui/blog.git
cd blog
git clone https://github.com/lijiarui/hexo-theme-jsimple themes/jsimple
```
## CODE INTRODUCTION

* this repo is blog backup and the source version.
* [lijiarui.github.io](https://github.com/lijiarui/lijiarui.github.io) is the generate part of the blog.

About username.github.io intro, see [here](http://warjiang.github.io/devcat/2016/02/24/%E5%A6%82%E4%BD%95%E5%88%A9%E7%94%A8githubpages%E6%9D%A5%E6%90%AD%E5%BB%BA%E8%87%AA%E5%B7%B1%E7%9A%84blog/)
* If use username.github.io, choose master
* Or, choose gh-pages branch

## DEPLOYING WITH TRAVIS
1. Add `travils.yml` and install travis
```
gem install travis
travis login
```
2. run `npm install --save hexo-deployer-git
`
3. get [Personal Access Tokens](https://github.com/settings/tokens)
4. add encrypt token using the following command and add encrypt token to `.travis.yml` automatically
```
travis encrypt 'GH_TOKEN=<TOKEN>' --add
```
5. Start [Travis CI](https://travis-ci.org) 

see more 
* [Deploying Hexo to Github Pages with Travis](https://sazzer.github.io/blog/2015/05/04/Deploying-Hexo-to-Github-Pages-with-Travis/)
* [Hexo-Auto-Deploy-to-Github](http://lotabout.me/2016/Hexo-Auto-Deploy-to-Github/)
* [手把手教从零开始在GitHub上使用Hexo搭建博客教程(四)-使用Travis自动部署Hexo](https://zhuanlan.zhihu.com/p/22405971)
