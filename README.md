![Version](https://img.shields.io/badge/Version-V24.8.240828144-red)
# Docker AWVS
基于Pwn3rzs license和Ubuntu 18.04手动制作的docker awvs版本
# Latest version: AWVS v24.8.240828144
# Usage:
- docker pull 0xgkd/awvs
- docker run -it -d -p 13443:3443 0xgkd/awvs
# Login Credentials:
- username: admin@gkd.com
- password: Oxgkd123
# Update:
- 2024.09.09 - AWVS v24.8.240828144
- 2024.07.15 - AWVS v24.6.240626115
- 2024.06.16 - AWVS v24.4.240514098
- 2024.06.03 - AWVS v24.4.240427095
- 2024.05.03 - AWVS v24.3.240322155(2024 五一假期特供版)
> 祝师傅们五一假期快乐！
- 2024.04.09 - AWVS v24.2.240226074
- 2024.03.01 - AWVS v24.1.240111130(8c152dacb50f)

- **~~2024.02.29 - AWVS v24.1.240111130~~**
> **v24.1.240111130官方移除了启动脚本，导致镜像f65c263bf9ba异常**
- 2024.01.17 - AWVS v23.11.231123131
- 2023.11.29 - AWVS v23.9.231020153
- 2023.10.19 - AWVS v23.9.231005181
- 2023.10.10 - AWVS v23.8.230905089
- 2023.08.25 - AWVS v23.7.230728157
- 2023.07.15 - AWVS v23.6.230628115
# Engine Update:
- 2024.10.16 - Engine v24.8.240828144
# Feature:
## Enable Multi-Engine
```
Step 1:
docker pull 0xgkd/awvs-engine:latest

Step 2:
docker run -it --name main -d 0xgkd/awvs:latest
docker run -it --name worker1 -d 0xgkd/awvs-engine:latest

Step 3:
docker inspect -f '{{.Name}} - {{.NetworkSettings.IPAddress }}' $(docker ps -aq)
Example:
/worker1 - 192.168.215.3
/main - 192.168.215.2

Step 4:
Example:
Main Installation Address: https://192.168.215.2:3443
Worker1 Address: https://192.168.215.3:3443
```
# Image Size:
![image](https://github.com/0xgkd/awvs/blob/main/image.jpg)
![size](https://github.com/0xgkd/awvs/blob/main/size.jpg)
![engine](https://github.com/0xgkd/awvs/blob/main/engine.jpg)
# Multi-Engine Authorization
![authorization](https://github.com/0xgkd/awvs/blob/main/authorization.jpg)
