# TempTake

## About

TempTake is a project based around IoT. The purpose of the project is to create a system that can monitor measurments like temperature, humidity, air pressure and PPM. These measurments are achieved by using the ESP32-C3 microcontroller the ENS160+AH21 and the BMP390 sensors. The data is stored in a database and can be accessed through a web interface.

## Installation and setup

### 1. Clone the main repository

```bash
git clone --recurse-submodules https://github.com/muffindud/TempTake
```

### 2. Update the submodules
```bash
git submodule update --remote --merge
```

### 3. Run the docker-compose file
(make sure you have docker and docker-compose installed and running)
```bash
docker-compose down && docker-compose build --pull && docker-compose up
```

### 4. Connect the Manager module
(follow the instructions in the [Manager README](./TempTake-Manager/README.md) and [Worker README](./TempTake-Worker/README.md))
