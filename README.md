# JavaFromSwagger
Generate java code from swagger api or json


# Swagger 代码生成工具使用
## 代码生成工具，项目GitHub地址
https://github.com/swagger-api/swagger-codegen
## 生成代码命令行
Java命令行，配置文件：[config.json](config.json)
```cmd
java -jar swagger-codegen-cli-2.4.13.jar generate -i FeHelper-20200421170753.json -o client -l java -c config.json
```
C#命令行，配置文件：[config_csharp.json](config_csharp.json)
```cmd
java -jar swagger-codegen-cli-2.4.13.jar generate -i FeHelper-20200421170753.json -o client -l csharp -c config_csharp.json
```

## 命令行帮助
```cmd
java -jar swagger-codegen-cli-2.4.13.jar help	
```
## 生成命令行帮助
```cmd
java -jar swagger-codegen-cli-2.4.13.jar generate help
```
## 配置帮助命令
```cmd
java -jar swagger-codegen-cli-2.4.13.jar config-help -l java
```

## Gradle下载配置：
```groovy
implementation group: 'io.swagger', name: 'swagger-codegen-maven-plugin', version: '3.0.0-rc1'
implementation group: 'io.swagger', name: 'swagger-codegen-cli', version: '3.0.0-rc1'
implementation group: 'io.swagger', name: 'swagger-codegen-maven-plugin', version: '2.4.13'
implementation group: 'io.swagger', name: 'swagger-codegen-cli', version: '2.4.13'
```


## 参考资料
[Swagger Codegen 自动生成Retrofit 代码](https://juejin.im/entry/598d8eb86fb9a03c52459e2a)  
[Icon列表](https://jetbrains.design/intellij/resources/icons_list/)  
[你们要的Intellij IDEA 插件开发秘籍，来了！](https://cloud.tencent.com/developer/article/1348741)  

# Idea插件开发
## 1. 安装插件[gradle-intellij-plugin](https://github.com/JetBrains/gradle-intellij-plugin/)

## 2. 下载Idea社区版本及源代码：
[社区版本下载地址](https://cache-redirector.jetbrains.com/www.jetbrains.com/intellij-repository/releases/com/jetbrains/intellij/idea/ideaIC/2020.1/ideaIC-2020.1.zip)  
[源代码下载地址](https://cache-redirector.jetbrains.com/www.jetbrains.com/intellij-repository/releases/com/jetbrains/intellij/idea/ideaIC/2020.1/ideaIC-2020.1-sources.jar)  
[GitHub地址](https://github.com/JetBrains/intellij-community/)  
[官方文档](https://www.jetbrains.org/intellij/sdk/docs/basics/plugin_structure.html)  

## 3. 配置使用本地IDEA,否则gradle插件会进行下载
配置环境变量
```cmd
IDEA_IC_HOME='本地IDEA所在的目录'
```
gradle使用环境变量
```groovy
intellij {
    localPath System.getenv('IDEA_IC_HOME')
}
```
## 4. [插件官方样例](https://github.com/JetBrains/intellij-sdk-docs/tree/master/code_samples)
