## **Level 5 → Level 6**

### **Goal**: Find a file with specific properties (size, owner, group).

This level required me to find a file that was 1033 bytes in size, not executable, and owned by a specific user. I used the `find` command:

```bash
find . -type f -size 1033c ! -executable
```

It pointed me to `./maybehere07/.file2`. I read it:

```bash
cat ./maybehere07/.file2
```

And got the password!

---