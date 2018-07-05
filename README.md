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



