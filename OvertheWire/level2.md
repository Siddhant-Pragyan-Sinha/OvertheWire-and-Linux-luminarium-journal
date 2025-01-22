## **Level 1 → Level 2**

### **Goal**: Read a file named `-`.

This one was a bit tricky because the file was named `-`, which is a special character in Linux. I tried using `cat -`, but it didn't work. After some Googling, I learned that I needed to use `./-` to specify the file:

```bash
cat ./-
```

And there it was—the password for the next level!

---