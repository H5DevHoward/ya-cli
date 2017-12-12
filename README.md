# ya-cli

Simple CLI for scaffolding Ya projects

## 安装

环境 : [Node.js](https://nodejs.org/en/download/) , npm 3.0+、 [Git](https://git-scm.com/).

```bash
npm install -g yz-cli
```

## 创建项目

在要创建项目的路径执行 ‘ya init’。

```bash
$ ya

  Usage: ya <command> [options]

  Options:

    -V, --version  output the version number
    -h, --help     output usage information

$ ya init

  Usage: ya-init [project-name]


  Options:

    -o, --offline  使用已经下载的本地模板
    --template [value] 选择使用的模板
    -i, --install  下载模板后自动安装依赖
    -h, --help     output usage information

$ ya update
  Usage: ya-update [project-name]

  Options:

    -h, --help          output usage information
    -o, --offline       使用本地模板
    --template [value]  选择使用的模板
    -i, --install       下载模板后自动安装依赖
```

### Examples:

创建 / 更新项目

```
$ ya init project1
```

在当前目录创建 / 更新项目

```
$ ya init
```

更新当前项目

```
$ ya update project1
```

在当前目录更新项目

```
$ ya update
```

使用本地模板 & 自动安装依赖

```
$ ya init project1 -i -o
```

## 模板

自定义模板无需发布到 npm，只需上传到 github 并通过 template 参数使用即可

```
$ ya init project1 --template q13/vue-spa-template
```
