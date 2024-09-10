## SYS_CONTEXT için USERENV Bağlamının İncelemesi ##

SYS_CONTEXT fonksiyonu, Oracle veritabanında oturum veya ortam bilgilerini almak için kullanılır. <br>
Bu fonksiyon, belirli bir bağlam adı ve öznitelik adı alır ve bu özniteliğin değerini döndürür. <br>
SYS_CONTEXT için kullanıcı ve oturum bilgilerini döndüren USERENV bağlamında ne gibi bilgiler elde edebileceğimizi inceleyeceğiz. <br>

Aşadağıdaki açıklamaları okuduktan sonra repoda yer alan SYS_CONTEXT_USERENV.sql dosyası ile ilgili verilere erişebilirsiniz. <br>

<br>

1. **SESSION_USER**: Oturumun kullanıcı adını döndürür.
   ```
   SYS_CONTEXT('USERENV', 'SESSION_USER')
   ```
   <br>
   
2. **SESSIONID**: Oturum kimliğini (Session ID) döndürür.
   ```
   SYS_CONTEXT('USERENV', 'SESSIONID')
   ```
   <br>
   
3. **IP_ADDRESS**: Kullanıcının IP adresini döndürür.
   ```
   SYS_CONTEXT('USERENV', 'IP_ADDRESS')
   ```
   <br>
   
4. **LANGUAGE**: Oturumun dil ayarını döndürür.
   ```
   SYS_CONTEXT('USERENV', 'LANGUAGE')
   ```
   <br>
   
5. **OS_USER**: İşletim sistemi kullanıcı adını döndürür.
   ```
   SYS_CONTEXT('USERENV', 'OS_USER')
   ```
   <br>
   
6. **TERMINAL**: Kullanıcının terminal adını döndürür.
   ```
   SYS_CONTEXT('USERENV', 'TERMINAL')
   ```
   <br>
   
7. **HOST**: Kullanıcının makine adını döndürür.
   ```
   SYS_CONTEXT('USERENV', 'HOST')
   ```
   <br>
   
8. **BG_JOB_ID**: Arka plan iş kimliğini döndürür.
   ```
   SYS_CONTEXT('USERENV', 'BG_JOB_ID')
   ```
   <br>
   
9. **MODULE**: Oturumun modül adını döndürür.
   ```
   SYS_CONTEXT('USERENV', 'MODULE')
   ```
   <br>
   
10. **ACTION**: Oturumun eylem adını döndürür.
    ```
    SYS_CONTEXT('USERENV', 'ACTION')
    ```
    <br>
    
11. **CLIENT_IDENTIFIER**: İstemci tanımlayıcısını döndürür.
    ```
    SYS_CONTEXT('USERENV', 'CLIENT_IDENTIFIER')
    ```
    <br>
    
12. **DB_NAME**: Veritabanı adını döndürür.
    ```
    SYS_CONTEXT('USERENV', 'DB_NAME')
    ```
    <br>
    
13. **CURRENT_USER**: Geçerli kullanıcı adını döndürür.
    ```
    SYS_CONTEXT('USERENV', 'CURRENT_USER')
    ```
    <br>
    
14. **SERVER_HOST**: Veritabanı sunucusunun ana bilgisayar adını döndürür.
    ```
    SYS_CONTEXT('USERENV', 'SERVER_HOST')
    ```
    <br>
    
15. **NLS_TERRITORY**: Oturumun bölgesel ayarlarını döndürür.
    ```
    SYS_CONTEXT('USERENV', 'NLS_TERRITORY')
    ```
    <br>
    
16. **SID**: Oturum kimliğini (Session ID) döndürür.
    ```
    SYS_CONTEXT('USERENV', 'SID')
    ```
    <br>
    
17. **CURRENT_SCHEMA**: Geçerli şema adını döndürür.
    ```
    SYS_CONTEXT('USERENV', 'CURRENT_SCHEMA')
    ```
    <br>
    
18. **CURRENT_EDITION_NAME**: Geçerli sürüm adını döndürür.
    ```
    SYS_CONTEXT('userenv', 'CURRENT_EDITION_NAME')
    ```
    <br>
    
19. **INSTANCE_NAME**: Veritabanı örneğinin adını döndürür. Üçüncü parametre olan `200`, döndürülen değerin maksimum uzunluğunu belirtir.
    ```
    SYS_CONTEXT('USERENV', 'INSTANCE_NAME', 200)
    ```
    <br>
