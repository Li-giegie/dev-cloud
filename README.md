# dev-cloud
## 云开发是一个帮助开发者在本地环境开发，远程运行、调试的工具。  

### 自述
侦查程序侦查到当前进行的项目有更新时，通知同步端进行同步，被同步端收到同步的数据和指令后首先写入更新，在完成接下来的指令调用。  
1.数据传输传输协议采用http协议  
2.数据结构包含更新、指令

### 结构
```
dev-cloud
│  go.mod
│  go.sum
│  main.go              启动文件
│  README.md            自述文件
├─cmd                   项目命令
│      rootCmd.go
├─dev-rsync             被同步端
│      .gitignore
│      main.go
└─dev-sync              同步端
    .gitignore
    main.go
```

### 分支
```
main                    主分支
devctl                  命令行分支
dev-rsync               被同步端分支
dev-sync                同步端分支
```