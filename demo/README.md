cmusphinx-mavenized: demo
===================

CMU Sphinx - Mavenized - Demo

### Intro

This dir contains sphinx demo applications.


### Demos

* Hello World more info (http://cmusphinx.sourceforge.net/sphinx4/src/apps/edu/cmu/sphinx/demo/helloworld/README.html)

### Acoustic model

If you want intall to maven repository more acoustic model you can use this command
	mvn install:install-file -Dfile=WSJ_8gau_13dCep_16k_40mel_130Hz_6800Hz.jar  -DgroupId=edu.cmu.sphinx.model -DartifactId=WSJ_8gau_13dCep_16k_40mel_130Hz_6800Hz -Dversion=1.0 -Dpackaging=jar
