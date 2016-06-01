##Failsafe


El plugin de maven para las pruebas de integracion es: Failsafe. Failsafe es un fork de surefire. 
La gran diferencia entre ambos plugins es que failsafe no fallara la construccion durante la fase de integration-test , esto posibilita que se ejecute la fase de post-integration-test
<!-- .element: class="fragment" --> 

Failsafe no esta activado por defecto, es necesario agregarlo al pom y configurarlo en los ciclos de vida correctos.
<!-- .element: class="fragment" --> 
```xml
<plugin>
  <groupId>org.apache.maven.plugins</groupId>
  <artifactId>maven-failsafe-plugin</artifactId>
  <version>2.19.1</version>
  <executions>
    <execution>
      <goals>
        <goal>integration-test</goal>
        <goal>verify</goal>
      </goals>
    </execution>
  </executions>
</plugin>
```
<!-- .element: class="fragment" --> 