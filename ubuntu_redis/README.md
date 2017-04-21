### What is it for?

Installs and configures a Redis server.

### Variables

#### ubuntu_redis_allowed_ips `Array`

IP addresses allowed to connect to our Redis server. By default servers listens on localhost so no firewall rules are necessary (except default UFW config).

example:

```yaml
ubuntu_redis_allowed_ips:
  - 127.0.0.1
```

#### ubuntu_redis_bind_address `String`

bind address a server will run on. By default server binds to localhost and is not accessible from outer world

default value:

```yaml
ubuntu_redis_bind_address: 127.0.0.1
```

#### ubuntu_redis_bind_port `String`

specifies a port server will listen for connections on

default value:

```yaml
ubuntu_redis_bind_port: 6379
```
