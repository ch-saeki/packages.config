# packages.config
1. PowerShellを管理者権限で起動。

2. 以下chocolateyインストールを実行。
```
Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1'))
```

3. packages.configのあるディレクトリに移動し、以下コマンド実行。
```
cinst ./packages.config
```
