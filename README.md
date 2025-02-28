![Version](https://img.shields.io/badge/Version-V25.1.250204093-red)
# Docker AWVS
Docker awvs version manually created based on Pwn3rzs license and Ubuntu 18.04
# Latest version: AWVS v25.1.250204093
# Usage:
- docker pull 0xgkd/awvs
- docker run -it -d -p 13443:3443 0xgkd/awvs
# Login Credentials:
- username: admin@gkd.com
- password: Oxgkd123
# Update:
- 2025.02.28 - AWVS v25.1.250204093
- 2024.11.28 - AWVS v24.10.241106172
- 2024.11.05 - AWVS v24.9.241015145
- 2024.09.09 - AWVS v24.8.240828144
- 2024.07.15 - AWVS v24.6.240626115
- 2024.06.16 - AWVS v24.4.240514098
- 2024.06.03 - AWVS v24.4.240427095
- 2024.05.03 - AWVS v24.3.240322155
- 2024.04.09 - AWVS v24.2.240226074
- 2024.03.01 - AWVS v24.1.240111130(8c152dacb50f)

- **~~2024.02.29 - AWVS v24.1.240111130~~**
> **v24.1240111130 official remove startup files caused image f65c263bf9ba abnormality, fixed in 8c152dacb50f**
- 2024.01.17 - AWVS v23.11.231123131
- 2023.11.29 - AWVS v23.9.231020153
- 2023.10.19 - AWVS v23.9.231005181
- 2023.10.10 - AWVS v23.8.230905089
- 2023.08.25 - AWVS v23.7.230728157
- 2023.07.15 - AWVS v23.6.230628115
# Engine Update:
- 2025.02.28 - Engine v25.1.250204093
- 2024.11.28 - Engine v24.10.241106172
- 2024.11.05 - Engine v24.9.241015145
- 2024.10.16 - Engine v24.8.240828144
# Multi-Engine:
```
Step 1: Pull Image
docker pull 0xgkd/awvs-engine

Step 2: Start Container
docker run -it -d -p 13443:3443 --name main 0xgkd/awvs
docker run -it -d -p 13446:3443 --name worker1 0xgkd/awvs-engine

Step 3: Confirm IP Address Of Container
docker inspect -f '{{.Name}} - {{.NetworkSettings.IPAddress }}' $(docker ps -aq)
Example:
/worker1 - 172.17.0.3
/main - 172.17.0.2

Step 4: Finish Registration
Access main and worker1 and use above ip address of container to fill in on the registration page
Example:
https://172.17.0.3:3443
https://172.17.0.2:3443
```
# Image Size:
![image](https://github.com/0xgkd/awvs/blob/main/image.jpg)
![size](https://github.com/0xgkd/awvs/blob/main/size.jpg)
![engine](https://github.com/0xgkd/awvs/blob/main/engine.jpg)
