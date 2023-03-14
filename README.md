# Custom-bossbar-addon ![ダウンロード](https://img.shields.io/github/downloads/Gotemba912/Custom-bossbar-addon/total?style=plastic)  
このアドオンは、ボスバーを自分で作ることができます!  

> ⚠注意  
> このアドオンを使用すると、バニラのボスバーやscoreboardのsidebarが使えなくなります。

★To view the English version of the README, please click here: [README_en.md](https://github.com/Gotemba912/Custom-bossbar-addon/blob/main/README_en.md)

# 使い方
リソースパックをワールドに適用したら、以下のコマンドを実行してobjectiveを作成してください。  
★`<ID>` には任意のIDを入れてください。
```
/scoreboard objectives add <ID> dummy
```
次に、sidebarに作ったobjectiveを表示してください。
```
/scoreboard objectives setdisplay sidebar <ID>
```

これで準備完了です!  
objectiveに任意の値を入れてみてください。  
画面上部にボスバーが表示されます!

# 最大値を設定する
デフォルトでは、範囲は 0～100 に設定されています。

最大値を変更したい場合は、  
パックのファイルを編集する必要があります。  
まず、`manifest.json`でUUIDを変更してください。  
※他のサーバーでこのパックが適用されている場合重複してしまうため。  

変更したら、 `ui` フォルダ内の `hud_screen.json` をテキストエディターで開きます。

34行目
```
"$bossbar_max_value": 100.0,
```
これが最大値を設定する箇所です。  
これを任意の値に設定しましょう。

> ⚠最大値を設定する際は、必ず .0 を付けてください。

設定の例:
```
"$bossbar_max_value": 32767.0,
```
変更したら忘れずに保存しましょう!

設定を適用するには、一度ワールドを抜けて入り直す必要があります。

# パックの使用
このパックは自由にあなたのパックへ組み込みできます。  
ただし、このパックからコピーされたことを表記する必要があります!

# ライセンス
[Licence.txt](https://github.com/Gotemba912/Custom-bossbar-addon/blob/main/Licence.txt)

# 製作者
@Gotemba912 (YukaYama0311)