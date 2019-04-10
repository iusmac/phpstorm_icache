# phpStorm – Improved Cache (ICache)
Is your phpStorm lagging or freezing sometimes? Or maybe you want to make it more fluid and faster? **No problem!** Just move its cache to RAM while it is in running! This bash script will help you to do it without thinking too much.
_(*) All the cache will be synchronized when phpStorm will be closed._

### Installation

1. Download and move the `phpstorm_icache.sh` to your desired location
2. Give the script `phpstorm_icache.sh` execute permission `chmod +x /path/to/phpstorm_icache.sh`
3. Change the `PHPSTORM_SH_PATH` and `PHPSTORM_CACHE_PATH` variables if you have different paths

### Usage
Instead of running the original `phpstorm.sh` use the `phpstorm_icache.sh`. That's all!

### NOTE

- You can still start the phpStorm from a desktop shortcut

```
[Desktop Entry]
...
Exec=/absolute/path/to/phpstorm_icache.sh
...
Terminal=false
...
```

- This script can probably work with other Jetbrains IDEs... Try to do it and inform me.

### Tested on
- Ubuntu 18.04 LTS
- phpStorm 2018.1
### Helpful
For the first starts it is recommended to leave the notifications active to ensure correct execution. To disable it edit the `SHOW_NOTIFICATIONS` variable.
For the unclear behavior if you are not using the terminal look at the log file in `PHPSTORM_CACHE_PATH/ICache-logs.log`
