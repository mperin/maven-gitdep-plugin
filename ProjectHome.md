**maven-gitdep-plugin** lets you specify a **GIT** repository and
hash as a dependency in **Maven**.

To use the plugin, add the following to your POM:

```
<dependencies>
    <dependency>
        <groupId>some.groupId</groupId>
        <artifactId>some.artifactId</artifactId>
        <version>version to check out</version>
    </dependency>
</dependencies>

<plugins>
    <plugin>
        <groupId>com.ejwa</groupId>
        <artifactId>maven-gitdep-plugin</artifactId>
        <version>0.1</version>
        <configuration>
            <gitDependencies>
                <gitDependency>
                    <groupId>some.groupId</groupId>
                    <artifactId>some.artifactId</artifactId>
                    <location>full URL to git repository</location>
                    <branch>master</branch>
                </gitDependency>
            </gitDependencies>
        </configuration>
    </plugin>
</plugins>
```