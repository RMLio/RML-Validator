RML-Validator
=============

Validator for [R2]RML mapping documents. 

It is implemented in Java based on [RDFUnit](https://github.com/AKSW/RDFUnit) test cases applied to mappings defined with [RML](http://rml.io/).

Clone
-----

You can clone the RML- Validator (and its subprojects)

    git clone https://github.com/RMLio/RML-Validator.git

Installation
------------

You can install RML-Validator using Maven, so make sure you have installed it first: http://maven.apache.org/download.cgi and java 1.7

    bin/RML-Validator

Usage
-----

The RML-Validator can be run using Maven. You can run a validation process by executing the following command.
    
    mvn exec:java -Dexec.args=-m "<mapping_file> [-mqa -dqa -mdqa]"

Or using the JAR file

    java -jar RMLValidator-1.0.jar -m "<mapping_file> [-mqa -dqa -mdqa]"

With 
    
    <mapping_file> = The RML mapping file conform with the [RML specification](http://semweb.mmlab.be/ns/rml)
    -mqa = Triggers the Mapping Quality Assessment (the RML mapping document conform with skolemized and inferred statements).
    -dqa = Triggers the RDF Dataset Quality Assessment.
    -mdqa = Triggers both the Mapping and the RDF Dataset Quality Assessment.
    add -V to validate it using RDFUnit	
        
Remark
-----

On OSX, it might be needed to export JAVA_HOME=$(/usr/libexec/java_home)

More Information
----------------

More information about the solution can be found at http://rml.io

This application is developed by Multimedia Lab http://www.mmlab.be

Copyright 2015, Multimedia Lab - Ghent University - iMinds

License
-------

The RML-Validator is released under the terms of the [MIT license](http://opensource.org/licenses/mit-license.html).
