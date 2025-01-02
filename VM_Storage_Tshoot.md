### **Path Connection Checking**

1. **Install UltraPath Console:(Window)**  
   First, ensure that you have installed UltraPath Console. You can download it from the official Huawei support page:  
   [UltraPath Console Installation Guide](https://support.huawei.com/enterprise/en/storage/ultrapath-pid-8576127/software/)
   - (https://support.huawei.com/enterprise/en/doc/EDOC1000105151/b710b47f/introduction-to-ultrapath-console)
   - Ultrapath User Guide: (https://wiki.colobridge.net/_media/%D0%BA%D0%B0%D1%82%D0%B0%D0%BB%D0%BE%D0%B3_%D1%81%D1%82%D0%B0%D1%82%D0%B5%D0%B9/%D1%84%D0%B0%D0%B9%D0%BB%D0%BE%D0%B2%D1%8B%D0%B5_%D1%81%D0%B8%D1%81%D1%82%D0%B5%D0%BC%D1%8B/oceanstor_ultrapath_for_windows_21.2.0_user_guide_01.pdf)

3. **Launch UltraPath Console:**
   - Press `Win + R` to open the Run dialog box.
   - Type `ultrapath` and press Enter. This should open the UltraPath Console if the software is installed.

4. **Verify Installation:**
   - If `ultrapath` doesn’t open, check if the software is installed. You can search for it in the Start menu or navigate to the installation directory (usually located in `C:\Program Files (x86)\Emulex\UltraPath`).

5. **Open via Command Prompt (if needed):**
   - Open the Command Prompt (`cmd`) as an administrator.
   - Navigate to the UltraPath installation folder:
     ```bash
     cd C:\Program Files (x86)\Emulex\UltraPath
     ```
   - Run the UltraPath command:
     ```bash
     ultrapath.exe
     ```

6. **Check Link Status:**
   - Once the UltraPath Console is open, you should be able to view the status of your paths, controllers, and any link issues in the console window.


On a Linux host, you can check the status of physical paths by running the `upadmin show path` command.

- The "Path State" indicates the link status, where "Normal" means the path is functioning properly.

