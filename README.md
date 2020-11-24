# Cross Site Scripting Vulnerability on "Contact" feature in Lavelite.  
* Steps to reproduce the behavior:  
1. Log into the panel.  
2. Go to "/admin/contact/contact"  
3. Click "New" and Insert payload:  
"><img src=1 onerror=alert('xss')>  
4. Click "Save "  
5. View the preview to trigger XSS.  
6. View the preview to get in request and such Stored XSS  
Impact:Commonly include transmitting private data, like cookies or other session information, to the attacker, redirecting the victim to web content controlled by the attacker, or performing other malicious operations on the user’s machine under the guise of the vulnerable site.   

* POC:  
![image](https://github.com/BigTiger2020/Lavelite-CMS/blob/main/07.png)  
![image](https://github.com/BigTiger2020/Lavelite-CMS/blob/main/09.png)  
