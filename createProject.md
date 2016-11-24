# 创建mavne项目

1. 使用maven模板快速创建项目
```shell
    mvn archetype:generate -DgroupId=com.jianbingguozi.test -DartifactId=springmvc -DarchetypeArtifactId=maven-archetype-quickstart -DinteractiveMode=fase -X
    # -X 为打印日志
    # 这样创建项目会比较慢，原因是会从网络下载一个XXXX.xml（日志里名字，忘了...）文件。
    
    mvn archetype:create -DgroupId=com.jianbingguozi.test -DartifactId=springmvc -DarchetypeArtifactId=maven-archetype-quickstart -DinteractiveMode=fase -X
    # 创建项目较快
    # 与上一句好像没有什么区别
```
2. 个人喜好对创建的工程目录进行修改为适合web项目

```markdown
progect
└─┬ src
  ├─┬ main
  │ ├── java
  │ ├── resources
  │ └─┬ webapp
  │   ├── WEB-INF
  │   └── js,css,imgs...
  └─┬ test
    ├── java
    └── resources
```
3. [修改pom.xml文件构建项目](pomSetting.md)