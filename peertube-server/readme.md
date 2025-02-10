# Self Hosted PeerTube Server

This playbook allows you to self-host a PeerTube sever.

It was tested on Fedora 41.

Note: The playbook assumes that you bring your own webserver. You will need to configure a webserver either
on the machine you're installing PeerTube on or on another machine. 

My setup is as follows:

```mermaid
flowchart TD
    A[Internet] -->|Request| B(Reverse Proxy)
    B --> C(PeerTube Server)
```

Blogs:
- https://blog.nuculabs.dev/posts/2025/2025-01-25-self-hosting-peertube/
- https://docs.joinpeertube.org/install/docker

### Email

For e-mail, I use services from [Fastmail.com](https://join.fastmail.com/976cc1b5) on my custom domain.

I like it since it's budget friendly and
allows me to set up app passwords with SMTP access only (sending e-emails only as I share my Fastmail user with my
PeerTub server since it only needs to send emails not receive them).

You can get 10% off the first year if you use my referral link.
