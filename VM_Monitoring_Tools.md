### Linux

1. **Install `sysstat` package:**
   ```bash
   yum install sysstat
   ```

2. **Check CPU Info:**
   - To view CPU information:
     ```bash
     cat /proc/cpuinfo
     ```
   - Use `mpstat` for CPU statistics:
     ```bash
     mpstat
     ```

3. **Check System Performance:**
   - To monitor system performance:
     ```bash
     top
     ```
     (Press `1` to view individual CPU loading)
   
4. **Monitor Virtual Memory Statistics:**
   ```bash
   vmstat
   ```

5. **CPU Performance Analysis:**
   ```bash
   perf top --sort comm,dso
   ```

6. **Check Memory Usage:**
   ```bash
   free -h
   ```

7. **Clear System Cache:**
   ```bash
   sync
   echo 3 > /proc/sys/vm/drop_caches
   ```

8. **Check Disk I/O:**
   - To monitor disk I/O with a delay:
     ```bash
     iostat -d 3 3
     ```
   - For extended statistics:
     ```bash
     iostat -mx 1
     ```
   - To check I/O for a specific disk (e.g., `/dev/sdb`):
     ```bash
     iostat -d /dev/sdb
     ```

---

### Windows

1. **Performance Monitor:**
   - Search for "Performance Monitor" in the Start menu.
   - Click on the `+` symbol to add monitoring items.
   - Add **Physical Disk** for disk performance monitoring.

2. **Reliability Monitor:**
   - Navigate to:
     ```plaintext
     Control Panel\All Control Panel Items\Security and Maintenance\Reliability Monitor
     ```

3. **Storage Performance Monitoring:**
   - Open **Device Manager** to monitor storage devices.

---

This version is more structured and concise for easy understanding. Let me know if you need any further changes!
