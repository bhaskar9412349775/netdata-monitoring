# Task 7 – Monitor System Resources Using Netdata

## Objective
Deploy **Netdata** in Docker on Ubuntu to monitor real-time system metrics (CPU, memory, disk, containers) and explore its web dashboard.

---

## Steps Performed

### 1. Run Netdata container
```bash
docker run -d --name=netdata -p 19999:19999 netdata/netdata
 
```

