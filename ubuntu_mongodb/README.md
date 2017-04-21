### What is it for?

Installs and configures MongoDB server. At the moment only single instance (no replica set nor shard) is supported. 

### Variables

#### ubuntu_mongodb_allowed_ips `Array`

IP addresses allowed to connect to mongoDB server. By default server (firewall)
will allow connections from `localhost` and drop not allowed connections.

example:

```yaml
ubuntu_mongodb_allowed_ips:
  - 127.0.0.1
```

#### ubuntu_mongodb_data_dir `String`

directory where database data will be stored

default value:

```yaml
ubuntu_mongodb_data_dir: /var/lib/mongodb
```

#### ubuntu_mongodb_log_dir `String`

directory where server logs will be stored

default value:

```yaml
ubuntu_mongodb_log_dir: /var/log/mongodb
```

#### ubuntu_mongodb_bind_address `String`

bind address a server will run on. By default server binds to localhost and is not accessible from outer world

default value:

```yaml
ubuntu_mongodb_bind_address: 127.0.0.1
```

#### ubuntu_mongodb_bind_port `String`

specifies a port server will listen for connections on

default value:

```yaml
ubuntu_mongodb_bind_port: 27017
```
