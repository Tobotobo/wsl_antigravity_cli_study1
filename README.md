# wsl_antigravity_cli_study1

## 概要

* WSL を使って Antigravity CLI の実行環境を構築する
* root 権限を与えない
* Windows 側のフォルダの自動マウントを OFF にする

## 詳細

### 目次
* 環境構築
* 起動
* 削除

### 環境構築
```
$n="AlmaLinux-10-Antigravity"; wsl --install AlmaLinux-10 --name $n --no-launch; wsl -u root -d $n -- ./setup.sh; wsl -t $n
```

### 起動
```
wsl -d AlmaLinux-10-Antigravity
```

### 削除
```
wsl --unregister AlmaLinux-10-Antigravity
```

