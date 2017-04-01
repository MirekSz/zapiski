# zapiski

1. Podbicie hibernate
  Problem z wolnym startem spowodowanym parametrem hibernate.temp.use_jdbc_metadata_defaults
  
2. Podbicie JBossa
  Problem logera WARN vs WARNING oraz brak 2 wersji 7.1 
  ```xml
  <exclude-subsystems>
      <subsystem name="jaxrs" />
      <subsystem name="webservices" />
    </exclude-subsystems>
    ```
3. Dialog brak wpisów w DNS
4. NVision agent usuwający nagłówki GZIP
5. Pola nullable z JSON i reakcja na zmiane wartości pól w dataset
6. Visibility calendar i animacje CSS
7. Blokowanie INSERT INTO w PostgreSQL dla locków oraz indexów unikalnych
8. Hibernate cache cluster do deserailizacji wymagał  
```xml
<session-factory name="java:app/hibernate/SessionFactory"> 
```
9. Hawtio i wyciek pamięci na zapamiętaniu ostatnich 2000 logów
