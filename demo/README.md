cmusphinx-mavenized: demo
===================

CMU Sphinx - Mavenized - Demo

### Intro

This dir contains sphinx demo applications.


### Demos

*   sphinx4-hello_world - more info (http://cmusphinx.sourceforge.net/sphinx4/src/apps/edu/cmu/sphinx/demo/helloworld/README.html)
*   sphinx4-hello_world-lt - more info below in section _How put this into my maven project?_


### How put this into my maven project?

*   you should add repository where artifacts deployed:
	<repositories>
		<repository>
			<id>spnt-global-repo-release</id>
			<name>Spantus releases and 3rd party repo</name>
			<url>http://repository-spantus.forge.cloudbees.com/release/</url>
			<releases>
				<updatePolicy>daily</updatePolicy>
			</releases>
			<snapshots>
				<enabled>false</enabled>
			</snapshots>
		</repository>
	</repositories>
*   you should add sphix depenency :
		<dependency>
			<groupId>edu.cmu.sphinx</groupId>
			<artifactId>sphinx4</artifactId>
			<version>1.0.6</version>
		</dependency>
*   you should add sphix model :
		<dependency>
			<groupId>edu.cmu.sphinx.model.lt</groupId>
			<artifactId>lt.cd_cont_200</artifactId>
			<version>1.0</version>
		</dependency>
* you can add implementation based on sphinx.

### Acoustic model

If you want intall to maven repository more acoustic model you can use this command

	mvn install:install-file -Dfile=WSJ_8gau_13dCep_16k_40mel_130Hz_6800Hz.jar  -DgroupId=edu.cmu.sphinx.model -DartifactId=WSJ_8gau_13dCep_16k_40mel_130Hz_6800Hz -Dversion=1.0 -Dpackaging=jar
