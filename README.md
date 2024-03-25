# helm

helmfileを置くところ

## What is

* サービスの公開にはcloudflare tunnelを使っているよ
* 内部向けのサービスにはローカルDNSを構築しているよ
  - これはいずれ認証サーバを立てられてユーザ管理できるようになったら外部に公開するよ
* 適当に面白そうなサービスを載せてたりするよ
  - 2048
  - misskey
* secretファイルはsops暗号化しているよ

## Usage

```
$ helmfile -f {app-name}.yaml template
$ helmfile -f {app-name}.yaml diff
$ helmfile -f {app-name}.yaml sync
```
