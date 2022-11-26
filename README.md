# xmodmap-for-my-broken-hhkb-lite2

Fnキーが効かない私のHHKB Lite2をなんとか使えるようにするためのxmodmap設定

## Background

- 基盤が物理的に逝っていてFnキー(と↑キー)が効かない
	- Fn同時押しによる各種ファンクションキーが使えない
- 「右SuperとFnキーをスワップすればいいのでは？」と考えたがうまく行かなかった
	- **結論** 右SuperをFnキーに*見立て*、同時押しの設定を一つ一つ手動で行なう

## Usage

1. .Xmodmapファイルをホームディレクトリにコピー

```bash
git clone git@github.com:YUUKIToriyama/xmodmap-for-my-broken-hhkb-lite2.git
cd xmodmap-for-my-broken-hhkb-lite2
cp .Xmodmap ~/
```

 2. OS起動時に設定ファイルが読み込まれるよう設定

以下を`~/.xinputrc`に追記
```
if [ -f ~/.xmodmap ];then
  xmodmap ~/.xmodmap
fi
```

## Key bindings

| バインディング | 割り当て |
| - | - |
| [ | Up |
| ; | Left |
| ' | Right |
| / | Down |
| k | Home |
| l | Pg Up |
| , | End |
| . | Pg Down |
| 1 | F1 |
| 2 | F2 |
| 3 | F3 |
| 4 | F4 |
| 5 | F5 |
| 6 | F6 |
| 7 | F7 |
| 8 | F8 |
| 9 | F9 |
| 0 | F10 |
| - | F11 |
| = | F12 |
