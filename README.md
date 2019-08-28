# Autoban tool for v2ray

The tool is from [autoban.py in shadowsocks](https://github.com/shadowsocks/shadowsocks/tree/master/utils). Can be used to ban **"duplicated session id"** issue.

## Usage:

The usage is same with original one.

```
python autoban.py < [path to access.log]
```

Use -c to specify with how many failure times it should be considered as an attack. **Default is 2**.

To continue watching for the log file:

```
nohup tail -F [path to access.log] | python autoban.py >log 2>log &
```

Use with caution. Avoid to ban yourself.