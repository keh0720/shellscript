# Shell Script

## IF

null check
```
if [[ $CMD = *[!\ ]* ]]; then
     ..
else
     ..
fi
```

## awk

kill by pid
```
kill -9 $(ps -ef | grep -v awk | awk '/PROCESS NAME/ {print $2}')
```
delete via awk
```
find <directory path> -name <file name> | awk '{print "\""$0"\""}' | xargs rm
```
