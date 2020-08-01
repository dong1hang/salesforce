# salesforce
salesforce開発者初級　完全未経験に向け
## 汎用設定

### 言語設定
    railheadで勉強する時、順番にやって、間違いのに、ポイントを取られないことがある
    原因は言語は英語じゃないの可能性があるだ
    言語設定：「プロファイルを参照」→「設定」→「言語とタイムゾーン」
        地域（アメリカ合衆国）、言語（英語） →「保存」
    会社言語設定：「設定」→「会社の設定」→「組織情報」→「編集」→「地域の設定」
        地域（アメリカ合衆国）、言語（英語） →「保存」
            

### ユーザーログインIPアドレス設定
    開発する時、セキュリティを考えなくて、どこでも開発できるように、IPアドレス設定が必要と思う
    本番環境はお客様の要求を従う、設定する
    設定方法：「設定」→「ユーザー」→「ユーザー」→「システム管理者」→「ログインIPアドレスの制限」→「新規」
        開始IPアドレス（0.0.0.0）,終了IPアドレス（255.255.255.255） →「保存」
            
            
### IEブラウザを使用する設定
    salesforce開発環境はIEブラウザで行う方法
    設定方法：「設定」→「セキュリティ」→「セッションの設定」→Lightning Experience での IE11 の使用の延長
        （延長期間中に Lightning Experience で IE11 を使用することに同意する）をチェック　→「保存」



 セールスの重要オブジェクト紹介

 * Lead Capture (LEAD（リード、見込み客）): 
   > web(facebook,Twitterなど),inbound calls( tel,emailなど),Lists(Excelなど)からキャプチャする
* Account(取引先):
   > ２つ客の種類がある。Person Account(個人)　Business Account(会社)
* Opportunitity(商談):
   > セールスの機会。OpportunitityとAccountの関係｛N：1｝の例：ABCD会社（Business Account）とOpportunitity A,Opportunitity B,Opportunitity C.....
   > フェーズ：
   >>　Prospecting
   >>　Developing
   >>　Negotiation/Review
   >>　Closed/Won
   >>　Closed/Lost
 * Contact(取引先責任者):
   > ContactとAccountの関係｛N：1｝の例： ABCD会社（Business Account）とABCD会社のIT　大朗部長（Contact）,ABCD会社の営業　村田部長（Contact）......
 * Case(ケース)     
   > 顧客の質問、フィードバックまたは問題だ.以下は  Account-Contact-Case(関係)
   ![](https://github.com/dong1hang/salesforce/blob/master/Account-Contact-Case(relationship).png)
## salesforceのデータタイプと管理
　
 * MVC model,view,controller 　
 * object,record(レコード),field(フィールド):
 >> object: Standard Object(標準オブジェクト)、Custom Object(カスタム　オブジェクト)：API　NAMEは"_c"ネーミングする
    
        
 　　
 

            

