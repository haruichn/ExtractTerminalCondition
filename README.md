# 軸補正ツール
HASCデータを「端末の位置(TerminalPosition)と固定状況(TerminalMount)」から抽出するプログラム

## 使い方
#### IntelliJ IDEAから使う場合
1. このプロジェクトを読み込む
2. dataディレクトリにHASCコーパスのデータを入れる.
3. 実行
4. outputディレクトリが作成され, そこに補正されたデータが出力される.

#### コマンドラインから使う場合
1. ExtractTerminalPosition.javaを適当なティレクトリにコピー
2. ExtractTerminalPosition.javaがある階層にcdで移動
3. ExtractTerminalPosition.javaと同ディレクトリにdataディレクトリを用意.
4. dataディレクトリにHASCコーパスのデータを入れる.
5. 以下のコマンドを実行
6. outputディレクトリが作成され, そこに補正されたデータが出力される.

##### コマンド
```
javac ExtractTerminalCondition.java
java ExtractTerminalCondition
```


### データのディレクトリ構成
```
.  
data  
├── 1_stay  
│  ├── person0001  
│  │   ├── HASCXXXXXX-acc.csv  
│  │   ├── HASCXXXXXX-gyro.csv  
│  │   ├── HASCXXXXXX-mag.csv  
│  │   └── ...  
│  ├── person0002  
│  └── ...  
├── 2_walk  
│　├── person0001  
│　│   ├── HASCXXXXXX-acc.csv  
│　│   ├── HASCXXXXXX-gyro.csv  
│　│   ├── HASCXXXXXX-mag.csv  
│　│   └── ...  
│　├── person0002  
│　└── ...  
└── ...
```


### 　
Developed by icchi  
2016/03/25
