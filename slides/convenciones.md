##Convenciones

Por defecto el plugin :  <!-- .element: class="fragment" --> 

- Surefire ejecuta : <!-- .element: class="fragment" --> ```**/Test*.java, **/*Test.java, and **/*TestCase.java ``` <!-- .element: class="fragment" --> 
- Failsafe ejecuta : <!-- .element: class="fragment" --> ```**/IT*.java, **/*IT.java, and **/*ITCase.java ``` <!-- .element: class="fragment" --> 

Todas el codigo de las pruebas debe estar en : src/test/java <!-- .element: class="fragment" --> 

Para ejecutar pruebas : <!-- .element: class="fragment" --> 
- Unitarias : mvn test <!-- .element: class="fragment" -->  
- Integracion : mvn verify <!-- .element: class="fragment" --> 
