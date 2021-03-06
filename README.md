Maven archetype which is used to generate Aion AVM based smart contract project in java.

## Usage:

```
$> mvn archetype:generate -DarchetypeGroupId=org.aion4j -DarchetypeArtifactId=avm-archetype -DarchetypeVersion=<avm_archetype_version>
```

### Current archetype version: 0.30

To customize, contract class name, pass -DcontractName argument.
```
$> mvn archetype:generate -DarchetypeGroupId=org.aion4j -DarchetypeArtifactId=avm-archetype -DarchetypeVersion=0.30 -DcontractName=CounterContract
```

- In the generated project's pom.xml, change **aion4j.plugin.version** property to latest version of [aion4j-maven-plugin](https://github.com/bloxbean/aion4j-maven-plugin)

- To enable class verification for allowed classes in contract, uncomment **class-verifier** goal in pom.xml.
