Hi Alice,

I understand the urgency of getting your website back online. Here are some steps to diagnose and possibly resolve the issue:

### 1. Check Server Status
Firstly, ensure that the server at IP address 120.138.30.179 is running and accessible. You can do this by pinging the server:

1. **Ping the Server**:
   - Open a command prompt or terminal.
   - Type `ping 120.138.30.179` and press Enter.

If the server responds, it means the server is online. If it doesn't, there may be an issue with the server itself or network connectivity.

### 2. Check DNS Configuration
Ensure that the DNS records for `site.recruitment.shq.nz` are correctly configured. You can use online tools like `nslookup` or `dig` to verify this.

1. **Using nslookup**:
   - Open a command prompt or terminal.
   - Type `nslookup site.recruitment.shq.nz` and press Enter.
   - Ensure the returned IP address matches `120.138.30.179`.

### 3. Check for SSL/TLS Certificate Issues
The error message indicates a potential issue with the SSL/TLS certificate. Ensure that your certificate is correctly configured and has not expired.

1. **Verify Certificate Validity**:
   - Use an online tool like [SSL Labs](https://www.ssllabs.com/ssltest/) to test the SSL/TLS configuration of your site.

### 4. Check Web Server Configuration
Ensure that the web server (e.g., Apache, Nginx) on the server at `120.138.30.179` is running and correctly configured.

1. **Restart Web Server**:
   - Log in to your server via SSH.
   - For Apache: `sudo systemctl restart apache2`
   - For Nginx: `sudo systemctl restart nginx`

### 5. Check Firewall and Security Groups
Ensure that your server's firewall or security groups are not blocking HTTP/HTTPS traffic.

1. **Verify Firewall Rules**:
   - Check the firewall rules on your server to ensure ports 80 (HTTP) and 443 (HTTPS) are open.

### 6. Check Application Logs
Examine the web server and application logs for any error messages that could provide more insight into the issue.

1. **Apache Logs**:
   - `sudo tail -f /var/log/apache2/error.log`

2. **Nginx Logs**:
   - `sudo tail -f /var/log/nginx/error.log`

### Summary of Steps:
1. Ping the server to check if it's online.
2. Verify DNS configuration.
3. Check SSL/TLS certificate validity.
4. Restart the web server.
5. Verify firewall rules.
6. Examine web server and application logs.

By following these steps, you should be able to identify and resolve the issue preventing your website from being accessible.

If you need further assistance, please let me know.

Best regards,
Lanka Snehitha
