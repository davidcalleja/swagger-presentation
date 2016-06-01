## Ciclo de vida de maven

Como se ve las pruebas unitarias son una parte importante en ciclo de vida.  Si se ejecuta :
mvn package o mvn deploy se entrara tambien la fase de pruebas.<!-- .element: class="fragment" --> 

Porque ?  <!-- .element: class="fragment" -->   Por que en el [built-in Lifecycle Bindings](http://maven.apache.org/guides/introduction/introduction-to-the-lifecycle.html#Built-in_Lifecycle_Bindings) <!-- .element: class="fragment" -->  , la fase de pruebas esta ligada al plugin de surefire. <!-- .element: class="fragment" --> 

Surefire esta diseñado para ejecutar pruebas unitarias y si alguna de las pruebas falla la construccion fallara inmediatamente.<!-- .element: class="fragment" --> 

