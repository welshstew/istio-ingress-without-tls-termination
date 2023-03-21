```
openssl req -x509 -sha256 -nodes -days 365 -newkey rsa:2048 -subj '/O=example Inc./CN=example.com' -keyout example_certs/example.com.key -out example_certs/example.com.crt

openssl req -out example_certs/nginx.example.com.csr -newkey rsa:2048 -nodes -keyout example_certs/nginx.example.com.key -subj "/CN=nginx.example.com/O=some organization"
```