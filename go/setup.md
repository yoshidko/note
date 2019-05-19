# インストール
```
brew install go

```

# 準備
```
1. 開発用ディレクトリ作成
mkdir -p ~/Documents/workspace/go/src

2. GOPATH/GOBINの設定
export GOPATH=$HOME/Documents/workspace/go/src
export GOBIN=$GOPATH/bin
if [ -x "`which go`" ]; then
    export PATH=$PATH:$GOBIN
fi
```
