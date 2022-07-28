hp@DESKTOP-K19KSKK MINGW64 ~
$ mkdir git-basic

hp@DESKTOP-K19KSKK MINGW64 ~
$ cd git-basic

hp@DESKTOP-K19KSKK MINGW64 ~/git-basic
$ touch first.txt

hp@DESKTOP-K19KSKK MINGW64 ~/git-basic
$ git init first.txt
fatal: cannot mkdir first.txt: File exists

hp@DESKTOP-K19KSKK MINGW64 ~/git-basic
$ git init .
Initialized empty Git repository in C:/Users/hp/git-basic/.git/

hp@DESKTOP-K19KSKK MINGW64 ~/git-basic (master)
$ git add .

hp@DESKTOP-K19KSKK MINGW64 ~/git-basic (master)
$ git commit -m "adding first.txt"
[master (root-commit) 8790547] adding first.txt
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 first.txt

hp@DESKTOP-K19KSKK MINGW64 ~/git-basic (master)
$ git log
commit 879054779dd0c85c040902bac950235e606f8858 (HEAD -> master)
Author: prof aboy <rayhanrfn0704@gmail.com>
Date:   Thu Jul 28 11:03:15 2022 +0700

    adding first.txt

hp@DESKTOP-K19KSKK MINGW64 ~/git-basic (master)
$ touch second.txt

hp@DESKTOP-K19KSKK MINGW64 ~/git-basic (master)
$ git add second.txt

hp@DESKTOP-K19KSKK MINGW64 ~/git-basic (master)
$ git commit -m "adding second.txt"
[master fbe4a1c] adding second.txt
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 second.txt

hp@DESKTOP-K19KSKK MINGW64 ~/git-basic (master)
$ rm first.txt

hp@DESKTOP-K19KSKK MINGW64 ~/git-basic (master)
$ git add .

hp@DESKTOP-K19KSKK MINGW64 ~/git-basic (master)
$ git commit -m "removing first.txt"
[master 8c6c369] removing first.txt
 1 file changed, 0 insertions(+), 0 deletions(-)
 delete mode 100644 first.txt

hp@DESKTOP-K19KSKK MINGW64 ~/git-basic (master)
$ git log
commit 8c6c369b5bd413c872b0d281d53d6aac196543d5 (HEAD -> master)
Author: prof aboy <rayhanrfn0704@gmail.com>
Date:   Thu Jul 28 11:06:15 2022 +0700

    removing first.txt

commit fbe4a1ca9d3aab411f9306ccc8132e0cee0087d8
Author: prof aboy <rayhanrfn0704@gmail.com>
Date:   Thu Jul 28 11:04:39 2022 +0700

    adding second.txt

commit 879054779dd0c85c040902bac950235e606f8858
Author: prof aboy <rayhanrfn0704@gmail.com>
Date:   Thu Jul 28 11:03:15 2022 +0700

    adding first.txt
