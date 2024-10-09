# SWE_2021_41_2024_2_week_6
Explains activities in week 4 and week 5

## Week 4: The Happy Number
https://github.com/Min0Gyu0Kang/SWE_2021_41_2024_2_week_4/blob/main/2020315118_KangMinGyu.ipynb <br>
Code completed in Colab to find the true or false value for when a number is a happy number under these circumstances:

1. Starting with any positive integer, replace the number by the sum of the squares of its digits.
2. Repeat the process until the number equals 1 (where it will stay), or it loops endlessly in a cycle which does not include 1.
3. Those numbers for which this process ends in 1 are happy.

---

## Week 5: Practicing Docker
![docker env](https://github.com/user-attachments/assets/4a3e6837-96d6-46bc-8ee4-b736c1d5d07a)

### Checking Ubuntu Release Version
```bash
docker exec ossp-container cat /etc/os-release
```
The code to check the release version for Ubuntu in the Docker image container being used (`ossp-container`).

### Checking Git Version
```bash
docker exec ossp-container git --version
```
The code to check the downloaded Git version in the Docker image container.

### Checking Python3 Version
```bash
docker exec ossp-container python3 --version
```
The code to check the downloaded Python3 version in the Docker image container.

### Checking Bind Mount Directory Path
```bash
docker inspect --format="{{ .HostConfig.Binds }}" ossp-container
```
The code to check the given path for the bind mount directory of the Docker container. The current bind path is from `ossp_host_dir` to `ossp_container_dir`.
