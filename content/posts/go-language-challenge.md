---
title: "Go Language Challenge"
date: 2020-07-11T22:47:08+03:00
draft: true
toc: false
images:
tags:
  - go
  - programming
  - vim
---

### Go Programlama

- Go ile neler yapabilirim diye ciktim bu yola bakalim ne cikicak.. Go kendi sitesinde yer alan tanimi ile baslayalim 

    > Go is an open source programming language that makes it easy to build **simple**, **reliable**, and **efficient** software.
- Tutorial uzerinden bu vurgulu kelimeleri dusunerek gecicem bakalim hangi durumlar icin evet dogru diyebilecegim. 


### Lokal Kurulumlar ve Vim Setup

Kendi resmi adresinden Go indirebilirsiniz [**https://golang.org**](https://golang.org) Editor olarak Vim kullanicagim. Gelismis IDE veya text editor kullanabilirsiniz ama olaya biraz daha derinden girismek icin VIM kullanmak iyidir ornek ekran goruntu belki ilginizi ceker :D. 

 <br></br>
!["Vim-Screen"](../../../../images/vim-example-screen.png)

Vim kurulumunu MacOS uzerinde yaptim windows nasil olur bilemem 
.vimrc dosyami ise github ![**Link**] ulasabilirsiniz. 

### Tutorial Incelemesi 1

Dokumanin ilk asamasi dilin sozdizimi uzerine ornekler olucak . 

#### Hello World!!

```Go
package main
import "fmt"

func main(){
    fmt.Println("Hello, World!!")
}
```
Ufak bir giris yaptik Go diline.  
