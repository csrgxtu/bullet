### bullet
chose best server or ip or host from a list of servers, and set the shadowsocks config file. i am doing this because i use shadowsocks service, and have a bunch of hosts, always need to chose the best server for my network, so i use ping's avg time as a Standard, the less the better.

#### usage
first, clone the repo
```bash
git clone https://github.com/csrgxtu/bullet.git
cd bullet
```

second, fill the server list you want to chose from in ping.py main method
```python

if __name__ == '__main__':
    addresses = ['server1', 'server2']
    set_best_shadowsocks('/path/to/shadowsocks/config/ss.json', addresses, 10)
```

third, use root run the script
```bash
sudo su
python ping.py
```

fourth, when done, the best server for shadowsocks will be in your shadowsocks config file
