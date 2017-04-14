修改部分
> * 修复乱码问题，生成文件一律转为utf-8
> * 修改配置catalog时，生成代码为Schema..table的问题
> * 修改生成注释类，将英文注释去掉，改为数据库字段注释
 mvn install -Dmaven.test.skip=true
 
 
 
 
 
 
 
 
 
 <plugin>
<groupId>org.mybatis.generator</groupId>
<artifactId>mybatis-generator-maven-plugin</artifactId>
<version>1.3.2</version>
<configuration>
<configurationFile>src/main/resources/generatorConfig.xml</configurationFile>
<verbose>true</verbose>
<overwrite>true</overwrite>
</configuration>
<dependencies>
<dependency>
<groupId>com.haier.hairy</groupId>
<artifactId>mybatis-generator-core</artifactId>
<version>1.0.1</version>
</dependency>
</dependencies>
</plugin>
