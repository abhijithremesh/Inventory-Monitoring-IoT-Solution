# SCION-IoT-Application
An IoT Application  implemented over SCION network 
SCION - SCALABILITY, CONTROL, AND ISOLATION ON NEXT-GENERATION NETWORKS.

SCION internet architecture feature's includes:
1. organizes existing ASes into groups of independent routing planes, called isolation domains, which interconnect to provide global connectivity.
2. Isolation domains provide natural isolation of routing failures and misconfigurations, give endpoints strong control for both inbound and outbound traffic.

The project involves the development of a smart pallet placing container system integrated with RFID module and a load cell which sends the article details over the SCION network and displays this information on a remote dashboard. 
1. A pallet containing a number of specific article is placed over the pallet container. The pallet is also attached with article's RFID      tag. 
2. The pallet container is assembled and integrated with a RFID module and a load cell interfaced together with raspberry pi.
3. The pallet container scans the RFID tag (RFID tag > RFID module > TCP > raspberry pi > SCION AS server)and measures the weight using the load cell (load cell > raspberry pi > SCION AS server ). This information is sent to the client on request.
   A SCION server AS is configured to send this info over the SCION network at the raspberry pi end.
4. At the client end, A SCION client AS is configured which generates request to the SCION AS server at the raspberry pi end. The response    is displayed on a remote dashboard specifying the article detais : name, unit weight, number of pieces etc.
