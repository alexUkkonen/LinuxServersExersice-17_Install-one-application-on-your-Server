# LinuxServersExersice-17_Install-one-application-on-your-Server

## 1. The name of the daemon

To find the name of the daemon we can ps grep ssh.

<img width="1919" height="147" alt="image" src="https://github.com/user-attachments/assets/2b3cc0ee-4d81-4a20-960a-066aec17655f" />

## 2. How can we check of the ssh-server is running?

Well we did that in the last exercise but we can also use `$ sudo systemctl status ssh` (or sshd depending on the linux distro)

<img width="884" height="405" alt="image" src="https://github.com/user-attachments/assets/b4e55bc0-05ba-420a-bac5-b76bf2da28f2" />

## 3. How do we restart ssh?

We can restart ssh the same way we started it and the same way we checked it's status using `$ sudo systemctl restart ssh`

## 4. How to find your IP?

Ther are 2 types of IP's (outside of IPV4 and IPV6) Externam and Internal

To find your internal IP (the IP assigned by your router and how devices on your network view you) you can use `hostname -I`

To find your externa IP (the IP assigned by your ISP and how devices outside your network see you) you can use the command `curl ifconfig.me`. As this IP isn't known by your device you need to ask an external server.
