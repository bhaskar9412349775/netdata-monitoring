# Task 7 – Monitor System Resources Using Netdata

## Objective
Deploy **Netdata** in Docker on Ubuntu to monitor real-time system metrics (CPU, memory, disk, containers) and explore its web dashboard.

---

## Steps Performed

### 1. Run Netdata container(This will create Netdata Docker Image)
```bash
docker run -d --name=netdata -p 19999:19999 netdata/netdata
```

### 2. To Verify container is running
```bash
docker ps
```

### 3. Access the dashboard
```bash
Local machine: http://localhost:19999
```

### 4. Explore metrics
```bash
    -System Overview (CPU, RAM, Load Average)

    -CPU detailed charts

    -Memory usage

    -Disks I/O charts

    -Containers metrics
```

### 5. Check logs
```bash
docker logs netdata --tail 50
#### inside Container
docker exec -it netdata bash
ls -l /var/log/netdata
```

### 6. Screenshots Available

### 7. Cleanup
```bash
docker stop netdata
docker rm netdata
```

# THANK YOU

