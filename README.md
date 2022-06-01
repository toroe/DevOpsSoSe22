# DevOpsSoSe22
Dieses Repository dient dem Zwecke der Dokumentation und Versionskontrolle des Abgabeprojektes für den Kurs DevOps.
## Projektbeschreibung
Im Zuge dieses Projektes wird eine Artikel retrieval Anwendung in einem Kubernetes Cluster deployed. Die Anwendung besteht aus drei Servicen: Ein Frontend Service auf Basis von Javascript. Dieser Service ist ein Webserver welcher eine Website auf einem spezifischen Port für Benutzer anbietet. Zu dem existiert ein Backend Service auf Basis von Python. Mit Hilfe der Python Library Fast API wird eine Backend API implementiert, welche die Verbindung zwischen dem Frontend Service und dem Persistency Service bildet. Der Persistency Service ist eine Graph-Datenbank auf Basis von Neo4j. In dieser Datenbank sind Wissenschaftliche Artikel hinterlegt, welche im Zuge des Use Cases retrieved werden.
## CI/CD Pipeline
Die Pipeline wird drei Prozesse beinhalten. Build / Test / Release. Angesprochen werden die jeweiligen Prozesse durchs pushen in die jeweiligen Branches. Der Build Prozess soll erstmal unabhängig von dem Testing und Releasing sein. Der Test Prozess ist ebenfalls erstmal unabhängig. Der Release Prozess setzt jedoch das erfolgreiche Builden und Testen der Codebase vorraus, bevor das Projekt in die Produktion veröffentlicht werden kann.
