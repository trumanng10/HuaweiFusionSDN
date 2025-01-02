To **import** or **export certificates** on a Huawei OceanStor storage system, including the **OceanStor 2624**, you typically use the system's CLI (Command Line Interface) for security and certificate management.

### **Exporting a Certificate**

If you're exporting a certificate (perhaps a public certificate or the whole certificate chain), you'd use a command like:

```bash
seccertmgmt export <certificate-name> <file-path>
```

Where:
- `<certificate-name>` is the name of the certificate you want to export.
- `<file-path>` is the location where you want to store the exported certificate.

Example:

```bash
seccertmgmt export my-cert /home/admin/my-cert.pem
```

This command would export the certificate named `my-cert` to a file at `/home/admin/my-cert.pem`.

### **Importing a Certificate**

To **import a certificate**, use the `seccertmgmt import` command. The general syntax is:

```bash
seccertmgmt import <certificate-file-path>
```

Where:
- `<certificate-file-path>` is the file path of the certificate you want to import.

Example:

```bash
seccertmgmt import /home/admin/my-cert.pem
```

This command would import the certificate from `/home/admin/my-cert.pem` to the system.

### **Additional Options:**
1. **Check the status of certificates:**
   ```bash
   seccertmgmt show
   ```
   This will show a list of certificates currently installed on the system.

2. **View certificate details:**
   ```bash
   seccertmgmt show <certificate-name>
   ```
   This will show details about a specific certificate, such as its validity, issuer, and expiration date.

---

These commands should help with managing certificates on the Huawei OceanStor 2624. Make sure to follow best practices in managing certificates, such as verifying the certificate's source and integrity before importing it into your storage system.

To import a certificate (such as the one you've exported from the Huawei OceanStor) into your browser, you generally follow these steps depending on the browser you're using. Below are instructions for the most common browsers.

### **1. Google Chrome**
1. Open **Google Chrome**.
2. Click on the three-dot menu in the top-right corner and select **Settings**.
3. Scroll down and click **Privacy and Security**.
4. Click **Security**.
5. Under the **Advanced** section, click on **Manage certificates** (you might have to scroll down).
6. In the **Certificates** window, go to the **Trusted Root Certification Authorities** tab.
7. Click **Import** to start the **Certificate Import Wizard**.
8. Browse and select the `.pem` or `.crt` certificate file you want to import.
9. Choose the **Place all certificates in the following store** option and select **Trusted Root Certification Authorities**.
10. Click **Next** and then **Finish**.
11. Restart Chrome to ensure the certificate is applied.

### **2. Mozilla Firefox**
1. Open **Mozilla Firefox**.
2. Click on the three horizontal lines (menu) in the top-right corner and select **Settings**.
3. Scroll down to the **Privacy & Security** section.
4. Scroll down to the **Certificates** section and click **View Certificates**.
5. In the **Certificate Manager**, click the **Import** button.
6. Browse and select the `.pem` or `.crt` certificate file you want to import.
7. Choose **Trust this CA to identify websites** (if it's a root certificate) and click **OK**.
8. Restart Firefox to apply the changes.

### **3. Microsoft Edge**
1. Open **Microsoft Edge**.
2. Click on the three-dot menu in the top-right corner and select **Settings**.
3. Scroll down and click **Privacy, search, and services**.
4. Scroll to the **Security** section and click **Manage certificates**.
5. In the **Certificates** window, go to the **Trusted Root Certification Authorities** tab.
6. Click **Import** and browse to the certificate file you want to import.
7. Select **Place all certificates in the following store** and choose **Trusted Root Certification Authorities**.
8. Complete the wizard and click **Finish**.
9. Restart Edge to apply the certificate.

### **4. Apple Safari**
1. Open **Safari** and go to **Applications** > **Keychain Access** (or search for it).
2. In **Keychain Access**, select **System** or **Login** depending on the certificate's use.
3. Drag the `.pem` or `.crt` certificate into the **Keychain Access** window, or click the **File** menu and select **Import Items**.
4. Select the certificate file and click **Open**.
5. Choose the keychain you want to store the certificate in (typically **System** or **Login**).
6. If it's a trusted root certificate, you may need to double-click it after importing, go to the **Trust** section, and set it to **Always Trust**.
7. Restart Safari to apply the changes.

### **General Notes:**
- Ensure that the certificate you’re importing is from a trusted source, as improperly importing certificates can leave you vulnerable to security risks.
- For iSCSI or SAN management systems, typically the **root certificates** or **server certificates** need to be imported into your browser for secure communication (HTTPS).

Once the certificate is successfully imported, you should be able to securely connect to the OceanStor system or other devices via HTTPS in your browser without warnings or errors.
