# Go 项目

这是一个简单的Go项目模板。

## 项目结构

```
.
├── main.go          # Go程序入口
├── go.mod           # Go模块定义
├── go.sum           # Go依赖版本锁定
├── .gitignore       # Git忽略文件
└── README.md        # 项目说明
```

## 快速开始

### 1. 初始化Go模块
```bash
go mod init example.com/myapp
```

### 2. 下载依赖
```bash
go mod download
```

### 3. 运行程序
```bash
go run main.go
```

### 4. 构建可执行文件
```bash
go build -o myapp
./myapp
```

## 环境要求

- Go 1.21 或更高版本

## 开发建议

- 遵循 [Go代码规范](https://golang.org/doc/effective_go)
- 使用 `go fmt` 格式化代码
- 使用 `go vet` 检查代码
- 使用 `golangci-lint` 进行代码检查

## 许可证

MIT
