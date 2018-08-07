Add a git remote in the Cloud9 console. Should look like this (replace the git url with your repo url):
```
git remote add origin git@github.com:C9Support/testPush.git
```
Add files and commit them: 
```
git add . 
git commit -m "First commit"
```
Push to github.You'll get an error:
```
git push -u origin master
Warning: Permanently added 'github.com,207.97.227.239' (RSA) to the list of known hosts.
Permission denied (publickey).
fatal: The remote end hung up unexpectedly
```
You can find your SSH key on your Cloud 9 Dashboard, on the right of the screen under Account Settings. Copy that and paste it into a new SSH entry on your GitHub account at https://github.com/settings/ssh.
Now everything goes smoothly:
```
yoenc9@demo_app:~/514754/demo_app (master) $ git push origin master
Counting objects: 104, done.
Delta compression using up to 2 threads.
Compressing objects: 100% (93/93), done.
Writing objects: 100% (104/104), 32.80 KiB, done.
Total 104 (delta 8), reused 0 (delta 0)
To git@github.com:yoengithub/c9-demo-app.git
 * [new branch]      master -> master
```

from: http://nereida.deioc.ull.es/~lpp/perlexamples/node770.html
