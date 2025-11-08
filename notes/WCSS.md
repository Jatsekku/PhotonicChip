# WCSS - Wrocław Centre for Networking and Supercomputing

# Supecomputer access

## SSH access and setup

https://man.e-science.pl/pl/kdm/dostep

```
ssh username@ui.wcss.pl
```

Username was given during registration. \
If you don't remember username/password you can use option "Forgot password" and provide an email, in response you'll get
link to reset password and username associaated with the e-mail.

Remember to protect your remote home directory!
```
chmod 700 ~
```

## Passwordless login
1. Generate ssh-key pair (skip if already have them)
```
ssh-keygen -t ed25519 -C "your_email@example.com"
```

2. Copy public key to remote WCSS server
```
ssh-copy-id -i ~/.ssh/id_ed25519.pub username@ui.wcss.pl
```

## Graphical access

https://man.e-science.pl/pl/kdm/oprogramowanie/openondemand

Graphical access is provided by web platform called "Open OnDemand".
The graphical interface itself is also provided via web interface.
It can be accesed here: https://ood.e-science.pl/

# Monitoring avilable resources
To check how much of resources has been used and how much of them left, run:

```
service-balance
```
