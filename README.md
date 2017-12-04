# FaceRecognitionSampleClientWeb. API Example:
***
Endpoint: **http://faces.idscan.net/upload.php**

Token is required: **“token”: “[Authentication Token]”**

# Methods:

* Analytics<br>
Upload one image in query body.
Returns the analytics after uploading the image.

POST-query example:

    POST /upload.php HTTP/1.1
    Host: faces.idscan.net
    Referer: http://faces.idscan.net/upload.php
    User-Agent: Mozilla
    Content-Type: multipart/form-data; boundary=-------------573cf973d5228
    Content-Length: 288
    Connection: keep-alive
    Keep-Alive: 300

    ---------------573cf973d5228
    Content-Disposition: form-data; name="file"; filename="1.jpg"
    Content-Type: image/jpeg

    Content file
    ---------------573cf973d5228--
    
---    
* Compare 2 images<br>
Upload two images in query body.
Returns match of the 2 images.

POST-query example: 

    POST /upload.php HTTP/1.1
    Host: faces.idscan.net
    Referer: http://faces.idscan.net/upload.php
    User-Agent: Mozilla
    Content-Type: multipart/form-data; boundary=-------------573cf973d5228
    Content-Length: 288
    Connection: keep-alive
    Keep-Alive: 300

    ---------------573cf973d5228
    Content-Disposition: form-data; name="file" filename="1.jpg"

    Content-Type: image/jpeg


    Content file
    ---------------573cf973d5228
    Content-Disposition: form-data; name="file2"; filename="2.jpg"
    Content-Type: image/jpeg

    Content file
    ---------------573cf973d5228--

Live demo <http://faces.idscan.net>
