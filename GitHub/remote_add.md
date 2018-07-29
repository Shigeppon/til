### ローカルに作成したgitリポジトリをgithubへpushする
https://qiita.com/koshihikari/items/dcf126fa9c0de2b6fa7e

### githubへpushするときに「Enter passphrase for key 」とpass phraseを聞かれる
.ssh/configへ以下を追加する
```
Host github.com
	AddKeysToAgent yes
	UseKeychain yes
	HostName github.com
	IdentityFile ~/.ssh/id_rsa.github
	User git
``` 