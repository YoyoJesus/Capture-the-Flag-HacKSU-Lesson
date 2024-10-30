# Description

I wonder what this really is... enc ''.join([chr((ord(flag[i]) << 8) + ord(flag[i + 1])) for i in range(0, len(flag), 2)])

# Solution

You could simply use [cyberchef](https://gchq.github.io/CyberChef/#recipe=Magic(3,true,true,'picoCTF')) on the `magic` setting, and get the flag </br>.

Or use this:
```py
decode = '灩捯䍔䙻ㄶ形楴獟楮獴㌴摟潦弸彥ㄴㅡて㝽'
print(decode.encode('utf-16-be'))
```