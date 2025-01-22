# **Level 6 → Level 7**

### **Goal**: Find a file owned by a specific user and group.

This level was a bit more challenging because I had to search the entire filesystem. I used the `find` command with some filters:

```bash
find / -user bandit7 -group bandit6 -size 33c 2>/dev/null
```

The `2>/dev/null` part suppressed error messages. I found the file at `/var/lib/dpkg/info/bandit7.password` and read it:

```bash
cat /var/lib/dpkg/info/bandit7.password
```

Password acquired!

---