## Python check for connectivity

```
$ sudo apt install python-systemd python3-systemd
$ virtualenv -p python3 env
$ source env/bin/activate
$ pip install -r requirements.txt
```

```
$ chmod 644 pi_network.service
$ sudo ln -s $(pwd)/pi_network.service /lib/systemd/system/pi_network.service
$ sudo systemctl daemon-reload
$ sudo systemctl enable pi_network.service
```
