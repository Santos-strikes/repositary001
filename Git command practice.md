santhoshkumar.t@CDK190 MINGW64 /d/Santhosh/Git (master)
$ git init
Reinitialized existing Git repository in D:/Santhosh/Git/.git/

santhoshkumar.t@CDK190 MINGW64 /d/Santhosh/Git (master)
$ git add demo01.html

santhoshkumar.t@CDK190 MINGW64 /d/Santhosh/Git (master)
$ git status
On branch master
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   demo01.html


santhoshkumar.t@CDK190 MINGW64 /d/Santhosh/Git (master)
$ git log
commit d0080ef8228e629e1b4ce0d4699ef723fccf8b98 (HEAD -> master)
Author: Santos-strikes <sktofficial868@gmail.com>
Date:   Mon Oct 9 17:00:53 2023 +0530

    Initial version 1.0

santhoshkumar.t@CDK190 MINGW64 /d/Santhosh/Git (master)
$ git add -A

santhoshkumar.t@CDK190 MINGW64 /d/Santhosh/Git (master)
$ git status
On branch master
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   1_zejqB99KHo0huYN3etCYGA.webp
        new file:   demo01.html


santhoshkumar.t@CDK190 MINGW64 /d/Santhosh/Git (master)
$ git commit -m "Initial version 2.0"
[master 2b10a1b] Initial version 2.0
 2 files changed, 7 insertions(+)
 create mode 100644 1_zejqB99KHo0huYN3etCYGA.webp
 create mode 100644 demo01.html

santhoshkumar.t@CDK190 MINGW64 /d/Santhosh/Git (master)
$ git log
commit 2b10a1b667bf29214c4c5233b47cdb63bf57b00a (HEAD -> master)
Author: Santos-strikes <sktofficial868@gmail.com>
Date:   Mon Oct 9 17:51:24 2023 +0530

    Initial version 2.0

commit d0080ef8228e629e1b4ce0d4699ef723fccf8b98
Author: Santos-strikes <sktofficial868@gmail.com>
Date:   Mon Oct 9 17:00:53 2023 +0530

    Initial version 1.0

santhoshkumar.t@CDK190 MINGW64 /d/Santhosh/Git (master)
$ git reset --hard ^C

santhoshkumar.t@CDK190 MINGW64 /d/Santhosh/Git (master)
$ git reset --hard d0080ef8228e629e1b4ce0d4699ef723fccf8b98
HEAD is now at d0080ef Initial version 1.0

santhoshkumar.t@CDK190 MINGW64 /d/Santhosh/Git (master)
$ git status
On branch master
nothing to commit, working tree clean

santhoshkumar.t@CDK190 MINGW64 /d/Santhosh/Git (master)
$ git reset --hard 2b10a1b667bf29214c4c5233b47cdb63bf57b00a
HEAD is now at 2b10a1b Initial version 2.0

santhoshkumar.t@CDK190 MINGW64 /d/Santhosh/Git (master)
$ git status
On branch master
nothing to commit, working tree clean

santhoshkumar.t@CDK190 MINGW64 /d/Santhosh/Git (master)
$ git reset --soft d0080ef8228e629e1b4ce0d4699ef723fccf8b98

santhoshkumar.t@CDK190 MINGW64 /d/Santhosh/Git (master)
$ git reset --soft 2b10a1b667bf29214c4c5233b47cdb63bf57b00a

santhoshkumar.t@CDK190 MINGW64 /d/Santhosh/Git (master)
$ git log
commit 2b10a1b667bf29214c4c5233b47cdb63bf57b00a (HEAD -> master)
Author: Santos-strikes <sktofficial868@gmail.com>
Date:   Mon Oct 9 17:51:24 2023 +0530

    Initial version 2.0

commit d0080ef8228e629e1b4ce0d4699ef723fccf8b98
Author: Santos-strikes <sktofficial868@gmail.com>
Date:   Mon Oct 9 17:00:53 2023 +0530

    Initial version 1.0
