# COMA Schema Matcher

This is a fork of the [COMA schema matcher](https://dbs.uni-leipzig.de/Research/coma.html)
(Code from [this]( https://svn.code.sf.net/p/coma-ce/mysvn/trunk coma-ce-mysvn) SVN repo)
modified for use in [BCNFStar](https://github.com/SchweizerischeBundesbahnen/BCNFStar).

## How to use


After building, you can execute this command from the root folder
```bash
 java -cp 'coma-engine/target/coma-engine-0.1-CE-SNAPSHOT-jar-with-dependencies.jar:lib/*' de.wdilab.coma.integration.COMA_API <source schema> <target schema> <match result location>
```

To execute it somewhere else, you need to copy all files mentioned in the classpath above,
i.e. all JARs in the `lib` folder, and `coma-engine/target/coma-engine-0.1-CE-SNAPSHOT-jar-with-dependencies.jar` (only exists after building)

## How to build

```bash
mvn install -DskipTests
```
