## **Level 0 → Level 1**

### **Goal**: Log into the game using SSH.

This was the first level, and it was pretty straightforward. I used SSH to connect to the server:

```bash
ssh bandit0@bandit.labs.overthewire.org -p 2220
```

The password for `bandit0` is `bandit0`. Once logged in, I found a file named `readme` in the home directory. I used the `cat` command to read it:

```bash
cat readme
```

The password for the next level was right there! Damn easy.

---