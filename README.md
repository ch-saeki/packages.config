# packages.config
1. PowerShellを管理者権限で起動。

1. 以下chocolateyインストールを実行。
```
Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1'))
```

1.以下インストールコマンド実行。(パスはその時に合わせて。)
```
cinst ./packages.config
```
