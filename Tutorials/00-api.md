# webpack2 API


## CLI

https://doc.webpack-china.org/api/cli/

https://doc.webpack-china.org/guides/get-started/


# 常用配置

## 列出命令行所有可用的配置选项

```sh
webpack --help
webpack -h
``` 

## 使用配置文件进行构建

指定其它的配置文件。
配置文件***默认***为 webpack.config.js，如果你想使用其它配置文件，可以加入这个参数。

```sh
webpack --config example.config.js
``` 
## 指定构建环境

传入 webpack 配置文件中使用的环境变量。

```sh
webpack --env.production    # 生产环境设置为 true
webpack --env.platform=web  # 平台设置为 "web"
``` 

## 以 JSON 格式输出 webpack 的运行结果

```sh
webpack --json
webpack --json > stats.json
``` 

在其他每个情况下，webpack 会打印一组统计信息，用于显示 bundle, chunk 和用时等详细信息。
使用此选项，输出可以是 JSON 对象。 
此输出文件(response)可被 webpack 的分析工具，或 chrisbateman 的 webpack 可视化工具，或 th0r 的 webpack bundle 分析工具接收后进行分析。 
分析工具将接收 JSON 并以图形形式提供构建的所有细节。



## configuration

https://doc.webpack-china.org/configuration/configuration-types

https://doc.webpack-china.org/configuration

```sh

``` 





