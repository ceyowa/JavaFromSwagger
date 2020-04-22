# JavaFromSwagger
Generate java code from swagger api or json

# 代码生成工具，项目GitHub地址
https://github.com/swagger-api/swagger-codegen


# 生成代码命令行
Java命令行，配置文件：[config.json](config.json)
```cmd
java -jar swagger-codegen-cli-2.4.13.jar generate -i FeHelper-20200421170753.json -o client -l java -c config.json
```
C#命令行，配置文件：[config_csharp.json](config_csharp.json)
```cmd
java -jar swagger-codegen-cli-2.4.13.jar generate -i FeHelper-20200421170753.json -o client -l csharp -c config_csharp.json
```

# 命令行帮助
```cmd
java -jar swagger-codegen-cli-2.4.13.jar help	
```
# 生成命令行帮助
```cmd
java -jar swagger-codegen-cli-2.4.13.jar generate help
```
# 配置帮助命令
```cmd
java -jar swagger-codegen-cli-2.4.13.jar config-help -l java
```

# Gradle下载配置：
```groovy
implementation group: 'io.swagger', name: 'swagger-codegen-maven-plugin', version: '3.0.0-rc1'
implementation group: 'io.swagger', name: 'swagger-codegen-cli', version: '3.0.0-rc1'
implementation group: 'io.swagger', name: 'swagger-codegen-maven-plugin', version: '2.4.13'
implementation group: 'io.swagger', name: 'swagger-codegen-cli', version: '2.4.13'
```


# 参考资料
[Swagger Codegen 自动生成Retrofit 代码](https://juejin.im/entry/598d8eb86fb9a03c52459e2a)


# Idea社区版本及源代码地址：
[社区版本下载地址](https://cache-redirector.jetbrains.com/www.jetbrains.com/intellij-repository/releases/com/jetbrains/intellij/idea/ideaIC/2020.1/ideaIC-2020.1.zip)

[源代码下载地址](https://cache-redirector.jetbrains.com/www.jetbrains.com/intellij-repository/releases/com/jetbrains/intellij/idea/ideaIC/2020.1/ideaIC-2020.1-sources.jar)

[GitHub地址](https://github.com/JetBrains/intellij-community/)
