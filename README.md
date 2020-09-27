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
10. Znikanjace pliki finalize DiskFileItem
11. CPU i Network blokady logiczne duzy modyfikowalny obiekt , cache copy-on-read i cluster multicast dużo modyfikacji invalidacji async
12. IE 11 startsWith('s') raz działa raz nie ramka i babel w parencie
13. EHcache
```
 WARN [net.sf.ehcache.distribution.RMIAsynchronousCacheReplicator] (Replication Thread) Unable to send message to remote peer due to socket read timeout. Consider increasing the socketTimeoutMillis setting in the cacheManagerPeerListenerFactory. Message was: Error unmarshaling return header; nested exception is:
java.net.SocketTimeoutException: Read timed out

WARN [net.sf.ehcache.distribution.RMIAsynchronousCacheReplicator] (Replication Thread) 2204678 messages were discarded on replicate due to reclamation of SoftReferences by the VM. Consider increasing the maximum heap size and/or setting the starting heap size to a higher value.

```
14. Hazelcast i niedziałający query cache https://github.com/hazelcast/hazelcast-hibernate5/issues/33
15. Groovy math i własny typ dziedziczący po number
16. SQLQuery w hibernate czysci wszystkie cache L2
17. Podwójny rozmiar w L2 https://github.com/hibernate/hibernate-orm/commit/954f1c4dfa5106b7914fc6c56a8202f119e5ff23#diff-d4e36c0df8cb46879a94c8a12b839384
18. Błąd
org.postgresql.util.PSQLException: ERROR: function prepare_account_report() does not exist
  Wskazówka: No function matches the given name and argument types. You might need to add explicit type casts.
problem z Boolean'ami na nowym sterowniku ten zrzut to popsuł 
https://github.com/pgjdbc/pgjdbc/commit/4942f7d1cc812feeeca331878334a3d4058615e4#diff-13f8af2e09f7a6b9b3e286e653aa63f7
poprawka springa https://github.com/spring-projects/spring-framework/commit/79ea77908ac3f68103d06935a0e2100621df988a#diff-0185284ff6b59ebc5d411260856366b4 ze względu na https://jira.spring.io/browse/SPR-15333
19. Hibernate błędy PK zabytanie hql w flush, zdarzenia
20. Hibernate orgomny IN https://github.com/hibernate/hibernate-orm/blob/39d9f84920081d3f110fca07ee30ca817f95d737/hibernate-core/src/main/java/org/hibernate/cfg/AvailableSettings.java IN_CLAUSE_PARAMETER_PADDING
21. Wiecej rdzeni wirtualnych niz fizycznych = stolen
22. WARNING [org.apache.cxf.jaxrs.provider.AbstractJAXBProvider] (default task-1) javax.xml.bind.UnmarshalException
  with linked exception:
[javax.xml.stream.XMLStreamException: Maximum Number of Child Elements limit (10) Exceeded]

WARNING [org.apache.cxf.jaxrs.impl.WebApplicationExceptionMapper] (default task-1) javax.ws.rs.WebApplicationException: HTTP 413 Request Entity Too Large

max-post-size attribute in the undertow subsystem: 10MB

23. Różna kolejność listenerów = deadlock, poprawa = select for update w kolejnosci = timeout na froncie (10 s i retry operacji). Szybki deadlock vs wolny lock. Wiele updateow tabela 100KB, a indeks 100GB, Vacummm freeze, reindex



