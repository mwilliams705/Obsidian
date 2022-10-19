Below is an example of the openapi-codegen-maven-plugin
```	xml	
	<plugin>
		<groupId>org.openapitools</groupId>
		<artifactId>openapi-generator-maven-plugin</artifactId>
		<version>6.0.1</version>
		<executions>  
		  <execution>  
			 <id>expense-business-api</id>  
			 <goals>  
				<goal>generate</goal>  
			 </goals>  
			 <configuration>  
<inputSpec>${project.basedir}/src/main/resources/openapi/ex-ms.yaml</inputSpec>  
<generatorName>spring</generatorName>            <modelPackage>com.snafusoft.service.business.EXAMPLE.openapi.model</modelPackage>              <apiPackage>com.snafusoft.service.domain.EXAMPLE.openapi.api</apiPackage>  
				<supportingFilesToGenerate>  
				   AppUtil.java  
				</supportingFilesToGenerate>  
				<configOptions>  
				   <delegatePattern>true</delegatePattern>  
				</configOptions>  
				<language>java</language>  
			 </configuration>  
		  </execution>  
	   </executions>  
	</plugin>
	```