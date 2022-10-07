## TailwindCSS

[https://github.com/matiu2/tailwind-yew-builder](https://github.com/matiu2/tailwind-yew-builder)を使用します.
導入方法はリンク先のREADMEを参照します. 

```bash
cd tailwind-yew-builder
docker-compose up dev
```

## Yew

ディレクトリ構成に関して[fullstack-rust](https://github.com/vascokk/fullstack-rust)というリポジトリを参考にしました.

`trunk`を使ってビルドします（自分用TODO: `trunk`を正しく理解する）

```bash
cd client
cargo install trunk wasm-bindgen-cli
trunk build -d ../server/static/ 
```

## Actix-web

```bash
cd server # 元のリポジトリの説明にあったcargoのオプションは不要かも
cargo run # --package server --bin server
```
