# goPortal
Captive Portal written in go

This is a light weight Captive portal designed for a rather special use case.
We need a solution to deploy hotspot networks which have to be fully seperated from the main infrastructure. This is an attampt at solving this issue.

The setup includes:
 - goPortal: The main application which hosts the Captive portal and also the endpoint for RFC8910
 - kea dhcp ipv4: Dhcp for the Lan network. Also sets dhcp option for RFC9810
 - Unbound as dns server

 Nedded is only Keycloak as external IDP
