# android studio初始化配置踩坑

## gradle 下载慢（右下角一直gradle download）
gradle 全局换源，修改或新建文件：~/.gradle/init.gradle
```
allprojects {
    repositories {
        maven {
            url "http://maven.aliyun.com/nexus/content/groups/public"
        }
    }
}
```
