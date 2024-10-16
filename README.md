# sensorHUB
The sensorHUB stack builds upon existing backend solutions from data management and IAM, and puts a new graphical web application into the center of the architecture, aiming to enhance the latest technology stack towards a novel, user-friendly IoT project solution. The sensorHUB’s graphical web application represents a new front-end application for managing IoT projects. Its streamlined navigation ensures sim plicity, allowing users to reach their intended destinations in a few clicks. 

The primary features include the management and visualization of IoT data. The app further provides a knowledge section, which includes essential training material on the provided software services. Interfaces to complementary IoT software (here: Node-RED) and optional forwarding of login tokens complement the default functionalities. Aligned with our requirements on interoperability, scalability and open-source, the data-related core of the sensorHUB stack represents a scalable cluster of Docker-containerized FROST-servers. 

The original sources of IoT data adding data to the FROST-Servers can be manifold; the post requests however need to fulfil the STA, which can be done directly from an external source or indirectly by transforming third-party data formats into STA using optionally provided instances of the Extract-Transform-Load (ETL)-software Node-RED (OpenJS Foundation, 2024). By integrating Keycloak into our application, we ensure that data and interactions are protected in accordance with users’ access rights. Keycloak provides authentication to the sensorHUB web application and secures its routes by requiring users to authenticate themselves. Due to its decentral approach, further modules implementing the required authentication interface
can be easily integrated. 

In addition, several supportive components were required to guarantee the scalability and func tioning of the network communication and server administration. Each sub-component is hosted as web application and can therefore be addressed using HTTP/S network communication. For mor details, see the related ISPRS publication: tba

![iot_stack_concept_finals2](https://github.com/user-attachments/assets/193af270-2ce4-46eb-857d-b68b87c6632f)

# Version
We provide two versions of sensorHUB:
- sensorHUB_LITE: a HTTP-based version for developing, testing and non-operational purposes on local machines (https://github.com/HEFLoRa/sensorHUB_LITE)
- sensorHUB_PRO: a HTTPS-based version for more operational uses with domain-based routes (https://github.com/HEFLoRa/sensorHUB_PRO)

Both versions, relate to the sensorHUB web application, which is separately provided: https://github.com/HEFLoRa/WEB_APP/
