# go-saml-test

## Get Started
### 1. Generate an self-signed X.509 key pair
```
openssl req -x509 -newkey rsa:2048 -keyout myservice.key -out myservice.cert -days 365 -nodes -subj "/CN=myservice.example.com"
```

### 2. Upload metadata
```
curl localhost:8000/saml/metadata > ./metadata.xml
```
Uploda `metadata.xml` from [this form](https://samltest.id/upload.php).

### 3. Access
Access to [http://localhost:8000/hello](http://localhost:8000/hello)
