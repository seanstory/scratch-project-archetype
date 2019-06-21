# JVM Sample Project Archetype

[![Build Status](https://travis-ci.org/seanstory/scratch-project-archetype.svg?branch=master)](https://travis-ci.org/seanstory/scratch-project-archetype)

### Overview

I find myself regularly re-building the same maven shell of a project. This will hopefully keep me from doing so again.

Projects built from this archetype will include:

* Java
* Groovy
* Kotlin
* Logback
* Slf4j
* Spock (testing)
* Junit (testing)

### Usage

1. First, build *this* project with `mvn clean install`
2. Then, in another directory, generate an "empty" project from the archtype with:

        
        mvn org.apache.maven.plugins:maven-archetype-plugin:2.4:generate \
        -DarchetypeGroupId=com.sstory.scratch \
        -DarchetypeArtifactId=scratch-project-archetype \
        -DarchetypeVersion=0.1.0-SNAPSHOT \
        -DgroupId=<your groupId> \
        -DartifactId=<your artifactId> \
        -Dversion=0.1.0-SNAPSHOT \
        -B
        
3. Enjoy your JVM development!