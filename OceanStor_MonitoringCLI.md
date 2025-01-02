Here are the OceanStor commands for monitoring, tidied up for clarity:

### OceanStor CLI Monitoring Commands

1. **Show Controller Information:**
   - To display controller information:
     ```bash
     show controller
     ```

2. **Show Performance of a Specific Controller:**
   - To display performance details for a specific controller (e.g., `controller_id=0A`):
     ```bash
     show performance controller controller_id=0A
     ```

3. **Show Port General Information:**
   - To display general port information:
     ```bash
     show port general
     ```

4. **Show Port General Information for a Specific Physical Type (e.g., Ethernet):**
   - To display the general information for Ethernet ports:
     ```bash
     show port general physical_type=ETH
     ```

5. **Show Performance of a Specific Port:**
   - To display performance statistics for a specific port (e.g., `port_id=CTE0.A.IOM4.P0`):
     ```bash
     show performance port port_id=CTE0.A.IOM4.P0
     ```

6. **Show Front-End I/O Information for a Specific Controller:**
   - To show front-end I/O statistics for a controller (e.g., `controller_id=0A`):
     ```bash
     show controller io io_type=frontEnd controller_id=0A
     ```

7. **Show LUN General Information:**
   - To display general information for a specific LUN (e.g., `LUN_OLTP_Linux`):
     ```bash
     show lun general lun_name=LUN_OLTP_Linux
     ```

---

These commands provide a good overview of the OceanStor system’s monitoring capabilities. Let me know if you need further elaboration!
