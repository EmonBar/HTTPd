# HTTPd

This is an implementation of our own HTTP server in a group of 2 people, following the HTTP/1.1 specification defined by the RFCs.

## Download

To download our project:

```
wget https://github.com/TRKirua/HTTPd.git -O "HTTPd.zip" &&
unzip ./"HTTPd.zip" &&
rm ./"HTTPd.zip"
```

## Compile

To compile our project:

```
make
```


## Usage

To run our project:

In one terminal launch the following command:

```
./httpd [--dry-run] [-a (start | stop | reload | restart)] server.conf
```

In another one launch your request with:

```
curl -i <ip> #GET
curl -i --head <ip> #HEAD
```

Or with:

```
echo -ne 'GET /<ip> HTTP/1.1\r\nHost: localhost\r\n\r\n' | nc localhost 4242 #GET
echo -ne 'HEAD /<ip> HTTP/1.1\r\nHost:
```

## Clean project

To clean the project:

```
make clean
```

## Credits :

- [BARBERIS Emon](https://github.com/EmonBar)
- [EKICI Enes](https://github.com/TRKirua)
