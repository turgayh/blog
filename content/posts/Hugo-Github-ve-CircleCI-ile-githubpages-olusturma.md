---
title: "Hugo Github ve CircleCI ile github-pages sayfasi olusturmak-[1]"
date: 2020-07-12T09:34:27+03:00
draft: true
toc: false
images:
tags:
  - Github
  - CircleCI
  - Automation
  - Pipline
  - Hugo Framework
  - Go Language
  - Blog
---
<br/><br/>
![Hugo FrameWork](../../../../images/hugo-framework.png)
<br/><br/>
**Hugo Framework :** Statik websitesi yapmanizi saglayan bir araci diye dusunebiliriz.Blog yazilari icin ideal bir ortam .Eger markdown ile blog yazarim ve herseyi kod kanaliyla yonetirim diyorsaniz uygun bir ortamdir.   

- Bu blog sayfasi da belirticegim yontemle calisiyor.Olabildigince islemleri otomatik hale getirdim . 

1. 2 farkli github reposu acilir, bunlardan biri github-pages olmali yani   [kullaniciadi.github.io] adresine icerik barindiracak repo olmali. 
[Bu adresten nasil olusturacaginiz yaziyor.](https://pages.github.com).  

2. Repo icersinde sadece README.md dosyalari kalmali eger varsa baska dosya silebilirsiniz .

3. Ben **blog** ve **turgayh.github.io**  diye 2 repo olusturdum.

4. Lokalde hugo projesini olusturalim . [Quick Start Hugo](https://gohugo.io/getting-started/quick-start/)

 ```shell
    hugo new site blog
 ```
blog reposunun icerigini olusturduk. 

```shell
cd blog
git init
git submodule add https://github.com/rhazdon/hugo-theme-hello-friend-ng.git themes/hello-friend-ng 
```
- Temayi submodule olarak git projemize ekledim . Beklenen themes klasoru altinda hello-friend-ng adinda temamizin gelmesi 
- **config.toml** dosyasi sitenizin ayarlar kismini barindiriyor. Bu dosya icerisinde temamizi belirtmek gereklidir ilk asamada themes/hello-friend-th/exampleSite  icersindeki config.toml icerigini kullanabiliriz.
```shell
    hugo new posts/my-first-post.md
```
- ilk blog postu ornegi md formatinda content/posts klasoru altinda olustur. 
```shell
hugo -D server
```
- Eger hersey yolunda gitmis ise [http://localhost:1313](http://localhost:1313)  alttaki ciktiyi alacaksiniz.  **blog** reposunu commit edebiliriz. 
-
![](../../../../images/hugo-example.png 'Ornek Tema ile sonuc')

