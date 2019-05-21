### Docker run
```
docker run \
-v $HOME/dev/online-judge/coderunner:$HOME/dev/online-judge/coderunner \
-v /usr/local/bin/docker:/usr/local/bin/docker \
-v /var/run/docker.sock:/var/run/docker.sock \
-w $HOME/dev/online-judge/coderunner \
-p 3000:3000 \
--rm -i -t node /bin/bash
```

### start coderunner
```
node app.js
```
