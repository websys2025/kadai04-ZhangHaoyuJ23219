## 自動販売機（オブジェクト、DOM、イベント処理）のミニレポート
### Q4-1. Itemクラスのメソッドについて説明せよ。
* showItemListがクラスメソッドである理由を考察せよ。
* buyItemがインスタンスメソッドである理由を考察せよ。
  
* showItemListは、全商品の情報をまとめて出力する処理であり、特定のインスタンスに依存しないため、クラスメソッドとして定義されている。一方、buyItemは在庫数を減らす処理であり、各インスタンスの状態に基づいて動作するため、インスタンスメソッドとして定義する必要がある。
* 
### Q4-2. 商品の購入ボタンをクリックすると、どのような処理でセルの値が減少するか説明せよ。
* 購入された商品の在庫数のセルをどのようにして特定するのか説明せよ。
* 特定したセルの値をどのように変更するのか説明せよ。

* 購入ボタンを押すと、該当商品のbuyItemメソッドが実行され、在庫数が1減少する。その後、在庫数のセルはID（"stockX"）で特定され、getElementByIdにより取得される。取得したセルのtextContentを書き換えることで、画面上の表示が更新される仕組みである。
* 
### Q4-3. 感想
* 今回の課題で苦労したこと
* 演習を通して理解できたこと
* この自動販売機プログラムの追加機能や課題など

* クラスメソッドとインスタンスメソッドの使い分けが難しく、特にstaticの意味を理解するのに苦労した。また、DOM要素とイベント処理を組み合わせて在庫数を更新する処理も複雑であった。今回の課題を通して、オブジェクト指向とDOM操作の基本を理解することができた。所持金を設定し、購入時に金額が足りない場合は購入できないような機能を追加したい。
