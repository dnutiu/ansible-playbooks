# OpenVPN + Obfs4 Server

This playbook automates the configuration of an OpenVPN + Obs4 server.

This is useful when you want to evade censorship and surveilance or just browse the web "privately".

After this playbook finishes executing you get a `user@ip` folder with the following files:

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

The `obfs4_bridgeline.txt` file will contain the obfs4's proxy cert key, that is used to communicate with the obfs4 proxy that's installed on the server.