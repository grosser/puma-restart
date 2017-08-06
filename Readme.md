Puma restart bug reproduction example.

```
bundle
bundle exec puma
... open new tab ...
ps -ef | grep puma
kill -SIGUSR2 <PID>
# puma should be restarted
```
