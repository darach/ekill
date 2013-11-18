ekill
=====

Kill an erl.

A simple shell script to kill a running distributed erlang node

# Example usage

If you have a ```${HOME}/.erlang.cookie``` that conflicts with the node on the distributed system
you would like to kill, then directly pass through a cookie:

```bash
$ ekill -sname sname@host -setcookie my_cookie
Killed sname@host
```

If you would like to kill a node from the configured distributed system
```bash
$ ekill -sname sname@host
Killed sname@host
```

If there is no known node to kill

```bash
$ ekill -sname sname@host
Unknown node: sname@host
```

