# Domain List to MRS Converter

这个项目用于将域名列表（.list文件）自动转换为 Mihomo 规则集（.mrs文件）。

## 功能特点

- 支持将 .list 格式的域名列表转换为 .mrs 格式
- 使用 GitHub Actions 自动化转换过程
- 当修改 .list 文件时自动触发转换

## 使用方法

1. 在 `rules` 目录下创建或修改 .list 文件
2. 文件格式要求：每行一个域名，支持以下格式：
   - 直接域名: example.com
   - 通配符域名: +.example.com
3. 提交更改后，GitHub Actions 将自动运行转换流程
4. 转换后的 .mrs 文件将自动生成在 `dist` 目录中

## 目录结构

```
.
├── rules/          # 存放原始 .list 文件
├── dist/           # 存放转换后的 .mrs 文件
└── .github/        # GitHub Actions 配置
``` 