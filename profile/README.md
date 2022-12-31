## Hi there 👋

### _SafeRoad_ is a system that allows localisation and visualization of potholes to monitor the quality of roads (we have too many in our ~~beloved~~ country Morocco).

![Web Application](./assets/amsa6-pothole-detection.jpg)

## The System Architecture

```mermaid
flowchart LR

    Frontend-->Backend;
    Backend-->Frontend;

    SmartThings--> Backend;
    id1[(Database)]<--->Backend;

```

![IoT System Architecture](./assets/iot-app-architecture.jpg)

we can break the system into 3 subsytems :

|              |          Frontend          |                     Backend                     |                         SmartThings                          |
| :----------: | :------------------------: | :---------------------------------------------: | :----------------------------------------------------------: |
|   Language   |         Javascript         |                   Javascript                    |                            Python                            |
| Technologies | Leaflet + Socket.io Client | NodeJS + ExpressJS + MongoDB + Socket.io Server | Requests + GPS + Raspberry PI + PI Camera + Huawei 4G Dongle |

# Demonstration Video

## [Demo Video](https://drive.google.com/file/d/1cuEcpcOaUutxG1opQEddCqUB-Nxv5CWZ/view?usp=sharing)
