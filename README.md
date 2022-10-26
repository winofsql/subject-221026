# subject-221026

### VSCode 用コードインストールバッチ

### 指定ファイルダウンロードスクリプト( VBScript )

```bat

mkdir ..\cs-core-mysql-01

cd ..\cs-core-mysql-01

dotnet new console -f net6.0

cscript C:\Users\%USERNAME%\AppData\Roaming\Code\User\script\download.vbs https://github.com/winofsql/cs-core-mysql-01/raw/main Program.cs

dotnet add package System.Data.Odbc

cscript C:\Users\%USERNAME%\AppData\Roaming\Code\User\script\workspace-build-download.vbs 2
```

### Git 利用
```bat
cd ..\

git clone https://github.com/winofsql/cs-con-odbc-access-select.git

cd cs-con-odbc-access-select

rmdir .git /S /Q

dotnet add package System.Data.Odbc

dotnet add package System.Data.OleDb

cscript C:\Users\%USERNAME%\AppData\Roaming\Code\User\script\workspace-build-download.vbs 2

```
