docker-compose stop

docker-compose up -d --build

注意:docker-compose.yml里面的目录映射

关于 go get的使用
如果您使用的 Go 版本是 1.13 及以上 （推荐）
	go env -w GO111MODULE=on
	go env -w GOPROXY=https://goproxy.cn,direct
  
关于go get 以后下载的包不在src下而在pkg的源头并且不可以import(Goland Modules模块的使用)  
在你需要导入第三方包的地方,打开终端输入go mod init 你先要的命名
然后在该文件夹会出现go.mod文件
然后使用go get 你想要导入的包地址
