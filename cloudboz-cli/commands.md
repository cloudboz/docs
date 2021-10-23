# Commands

These are the help texts for each of the core CloudBoz CLI commands. You can also see this text in your terminal with `cloudboz --help` or `cloudboz -h`.

## Databases

Database is an organized collection of data stored and accessed electronically from a computer system.

### MySQL

```
cloudboz create mysql:8.0
```

If you have an existing server, terminal will show this prompt. You can choose an existing server on your account or setup new server.

```
> Please Choose Server
- My Server 1
- Setup New Server
```

But, if you haven't any server, terminal will show this prompt. By default you will use CloudBoz Server for free trial.&#x20;

```
> It looks like that you haven't setup any server, please choose server provider
- CloudBoz Server (Free Trial) (default)
- Amazon Web Service
- Other
```

But, if you want to use your own Amazon Web Service account, please insert your API Key with full access to EC2. Please read this [documentations](https://docs.aws.amazon.com/IAM/latest/UserGuide/id\_credentials\_access-keys.html).

```
> Please Choose Server Provider
- CloudBoz Server (Free Trial) (default)
- Amazon Web Service
- Other

> Please Enter Your AWS API Key: 12309KASDFASD123

> Please Enter Your Server Name: MyServer
```

As an alternative option, you can choose Other. This option makes it possible to use another server provider like Google Cloud Platform, Azure, Vultr, DigitalOcean, etc. Please read this [requirements](../requirements.md).

```
> Please Choose Server Provider
- CloudBoz Server (Free Trial) (default)
- Amazon Web Service
- Other

> Please Choose How to Access Your Server
- Username & Password (default)
- Username & SSH Key

> Please Enter Your Access
- IP: 123.123.123.123
- Server Name: MyServer
- Username: root
- Password: ***********

> Please Enter Your Access
- Server Name: MyServer
- IP: 123.123.123.123
- Username: root
- SSH Key:
-----BEGIN OPENSSH PRIVATE KEY-----
Z7iXaCH6OIXUlQshS7ekDVjYolF55rsoYlzHg1fqir04yYm07YmZlNRBsTPSddSNeP7zqC
ji02OGmYIgYxLjLo5ofjXcmKdY/rSu8HiVhnsvt4YKADZaIbtQnu6e3RuYNeVEypGUF7xp
AUt9CTb5+AfKLPnPppvpEXL2IdT1o9vjgy+jc429hX6+azxm8amch/NzblFi9Z0MLwKcXH
A0EODqQ2ryrmMI/JO6lXKqKhcT/kFSKwAAAMEAw3CjzWtYVIDvJRyyBvZlJFdWRSkJgcFk
J/pjO2f3CkyfsqHzjROG0nK2bOZexteBKmXn6bF0zvRt+RBo76mjttieNXPotltJ4qo300
TTCHiDgOfiFJ2hj3a8RdZtZC4Bdty1Myj19gHVAmojJGXiYKnXeibNg5dIsMuYI+N4RomQ
Noz+cpJ8zkT/nofiAy2oOVH+RUs1FhLKVJ72cKvWE5mp6Siux5zi4dcisd5QYyxy0ms+At
EQPTmKD4WpjdhPAAAAE3N1Z2FuZGFAbWVtb29yYS5jb20BAgMEBQYH
-----END OPENSSH PRIVATE KEY-----
```

You can use existing servers, if you already connect your server with CloudBoz.

```
> Please Choose Server Provider
- CloudBoz Server (Free Trial) (default)
- Amazon Web Service
- Other
- Existing Servers

> Please Choose Existing Servers
- MyServer1
- MyServer2
- Back
```

### MariaDB

```
cloudboz create mariadb:8.0
```

### PostgreSQL

```
cloudboz create postgresql:8.0
```

### Cassandra

```
cloudboz create cassandra:8.0
```

### MongoDB

```
cloudboz create mariadb:8.0
```

## Web Server

Web server is computer software and underlying hardware that accepts requests via HTTP, the network protocol created to distribute web pages, or its secure variant HTTPS.

### Apache

```
cloudboz create apache:8.0
```

### Nginx

```
cloudboz create nginx:8.0
```

### OpenLiteSpeed

```
cloudboz create openlitespeed:8.0
```
