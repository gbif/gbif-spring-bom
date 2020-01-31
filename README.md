# GBIF BOM

List of dependencies and versions.

There are two ways how to use the GBIF BOM in a project:

 As a parent:
```
<project ...>
    <groupId>org.gbif</groupId>
    <artifactId>some-project</artifactId>
    <packaging>pom</packaging>
    <name>Some project</name>
    <parent>
        <groupId>org.gbif</groupId>
        <artifactId>gbif-bom</artifactId>
        <version>...</version>
    </parent>
</project>
```

 As a dependency:
```
<project ...>
    <groupId>org.gbif</groupId>
    <artifactId>some-project</artifactId>
    <packaging>pom</packaging>
    <name>Some project</name>
     
    <dependencyManagement>
        <dependencies>
            <dependency>
                <groupId>org.gbif</groupId>
                <artifactId>gbif-bom</artifactId>
                <version>...</version>
                <type>pom</type>
                <scope>import</scope>
            </dependency>
        </dependencies>
    </dependencyManagement>
</project>
```