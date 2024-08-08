# helm

helmfileを置くところ

## What is

* サービスの公開にはcloudflare tunnelを使っているよ
* 内部向けのサービスにはローカルDNSを構築しているよ
  - これはいずれ認証サーバを立てられてユーザ管理できるようになったら外部に公開するよ
* 適当に面白そうなサービスを載せてたりするよ
  - [2048.supaperman.net](https://2048.supaperman.net)
  - misskey (一時停止中)

## Build

```
$ helmfile -f {app-name}.yaml template
$ helmfile -f {app-name}.yaml diff
$ helmfile -f {app-name}.yaml sync
```
