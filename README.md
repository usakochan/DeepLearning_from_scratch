# コミットの仕方
初心者すぎるのでここから説明する。  
ディレクトリまで行った(cd)うえで...  
git add file.name #リモートリポジトリにプッシュしたいファイルをインデックスに追加  
git commit -m "何をしたか" #変更履歴を保存（コミット）する  
git push origin ブランチ名 #変更内容をリモートリポジトリにアップロード（プッシュ）する。デフォルトブランチならmain  

# 改めてリポジトリを作ったなら
https://qiita.com/mi-1109/items/006a534b26190424c499  
ここではSSHの設定の話がなくて手こずった。もうやったからTMDUnoMacbook-Airのローカルではやる必要はないんだけど。  
vs codeでsyncしないとremote/localでconflictを起こしてしまって手こずった。もうやったからただコミットすればいいんだけど。  
git init                                    #ディレクトリをgitで管理できるようにする（ローカルでgitを使えるようにする）  
git add hello.txt                           #リモートリポジトリにプッシュしたいファイルをインデックスに追加 (例：hello.txt)  
git commit -m "コミットメッセージ"            #変更履歴を保存（コミット）する。"コミットメッセージ"は日本語でもOK  
git branch -M main                          #デフォルト・ブランチ名をmasterからmainに変更（任意）  
git remote add origin リモートリポジトリURL   #originという名前でリモートリポジトリのURLを登録。URL部分はSTEP2でコピーしたURLを貼る。これでローカルとリモートが紐づく。  
git push origin ブランチ名                   #変更内容をリモートリポジトリにアップロード（プッシュ）する。デフォルト・ブランチをアップロードするなら、git push origin mainとなる  
