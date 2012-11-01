# Manually installing lpg.runtime.java [^why]
1. Download [lpg.runtime.java_2.0.18.jar](http://download.eclipse.org/technology/imp/updates/plugins/lpg.runtime.java_2.0.18.jar).
2. Install it to your local maven repository: 
> mvn install:install-file -DgroupId=lpg.runtime.java -DartifactId=lpg.runtime.java -Dversion=2.0.18 -Dpackaging=jar -Dfile=/path/to/lpg.runtime.java_2.0.18.jar

[^why]: The IMP repository is not yet a p2 repository. Thus, e.g. the required bundle *lpg.runtime.java;bundle-version="2.0.18”* cannot resolved via the tycho p2 target platform resolver.

# Go for it: Build your artefacts!
> mvn clean install