# Description

Using netcat (nc) is going to be pretty important. Can you connect to jupiter.challenges.picoctf.org at port 25103 to get the flag?

# Solution

As the problem statement has given us the host and the port, all we have to do is talk to it. Simply echo the message gotten when connecting to it using: 
```
echo | nc 2019shell1.picoctf.com 32225
```

We can plug that into the webshell that is available on the website directly, or you can use the command line on linux/mac