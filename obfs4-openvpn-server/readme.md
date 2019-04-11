# OpenVPN server + Obfs4

This playbook is configure multiple servers specified in the `hosts` file to act
as an OpenVPN server + obs4 proxy.

This is useful when you want to evade censorship and surveilance.

After this script finishes you get a `user@ip` folder in this folder with the following files:

```
├── root
│   └── client.ovpn
└── var
    └── lib
        └── tor
            └── pt_state
                └── obfs4
                    └── obfs4_bridgeline.txt
```

The `client.ovpn` file is the file that shall get imported into the OpenVPN client, before using this file you should change the port from 1194/tcp to 443/tcp.

The `obfs4_bridgeline.txt` file will contain the obfs4's proxy cert, that is used to communicate with
the obfs4 proxy that's installed on the server.