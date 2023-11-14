## Hi there 👋

### _SafeRoad_ is a system that allows localisation and visualization of potholes to monitor the quality of roads.

![Web Application](./assets/amsa6-pothole-detection.jpg)

## The System Architecture

```mermaid
flowchart LR

    Frontend--GET list of potholes-->Backend;
    Backend<--WebSockets new added pothole-->Frontend;
    Backend<-->id1[(MongoDB)];
    SmartThings--POST pothole position--> Backend;


```

<!--
![IoT System Architecture](./assets/iot-app-architecture.jpg)
-->

we can break the system into 3 subsytems :

|              |                      Frontend                       |                      Backend                       |                         SmartThings                          |
| :----------: | :-------------------------------------------------: | :------------------------------------------------: | :----------------------------------------------------------: |
|   Language   |                     Typescript                      |                     Javascript                     |                            Python                            |
| Technologies |             React + Leaflet + Socket.io Client              |  NodeJS + ExpressJS + MongoDB + Socket.io Server   | Requests + GPS + Raspberry PI + PI Camera + Huawei 4G Dongle |
|    Repo     | https://github.com/Potholes-ai/frontend-potholes-ai | https://github.com/Potholes-ai/backend-potholes-ai |   https://github.com/Potholes-ai/smart-things-potholes-ai    |

# Demonstration Video

## [Demo Video](https://drive.google.com/file/d/1cuEcpcOaUutxG1opQEddCqUB-Nxv5CWZ/view?usp=sharing)
