# trewys-oss

trewys-oss - trewys open source parent project object model


### References
---

[Sonatype OSS Manual](https://docs.sonatype.org/display/Repository/Sonatype+OSS+Maven+Repository+Usage+Guide)


### Release preparation
---

1. Make sure you put the proper sonatype release server settings into your ~/.m2/settings.xml
2. Make sure you own a verified gpg key (and still know the password ;) )
3. Make sure the build succeeds and the test coverage is acceptable


### Release
---

1. Clean your target, rebuild & test your code

        $ mvn clean install 


2. Prepare Release. Define the new version. Make SCM tag.

        $ mvn release:prepare


3. Perform release. Sign artifact and bring it out onto sonatype oss

        $ mvn release:perform


