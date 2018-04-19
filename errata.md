---
layout: default
title: "Microservices-Praxisbuch - Errata"
description: Errata für das Microservices-Praxisbuch
---

Errata
---

* 14.2.1 "Der Server ist ein WAR (Web Archive). Mit diesem WAR kann
  Eureka auf einem beliebigen Java-Webserver ausgeführt werden." Der
  Eureka-Server ist ein JAR. Eureka kann auch als WAR ausgeliefert
  werden. Das implementiert das Beispiel aber nicht.

* 15.8 "Sonst muss der Microservice explizit in Eureka gesucht
werden." Er müsste in *Consul* gesucht werden, nicht in Eureka.

* 15.8 "Erzeuge im docker-compose.yml einen Link vom Container mit dem
neuen Service zum Container eureka." Der Link muss zum Container
*consul* gehen, nicht eureka.

* 15.8 "Beobachte die Logs des Order-Microservice mit docker logs -f
ms_order_1" Der Container heißt *msconsul_order_1*.

* 17.3 Im Listing steht `kubectl run apache`. Es sollte `kubectl run
  catalog` heißen.
