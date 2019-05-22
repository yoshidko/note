# カレントディレクトリ内のDockerfileからDockerイメージ作成
```
docker build -t <tag> .
```

# マシン上の全てのDocker イメージ確認
```
docker images ls -a
```

# Docker イメージ削除
```
docker image rm <image id>
docker image rm -f $(docker image ls -a -q) // 全て強制的に削除
```

# マシンのポート4000をコンテナの公開ポート80に割り当ててコンテナの実行
```
docker run -p 4000:80 <Dockerイメージ名>
```
※バックグラウンドで実行する場合、-dオプション(detached option)で実行すれば良い

# コンテナを確認する
```
docker container ls
```

# プロセスを停止
```
docker stop <コンテナid>
```

