## **Level 3 → Level 4**

### **Goal**: Find a hidden file in a directory.

In this level, I had to find a hidden file in the `inhere` directory. I used `ls -la` to list all files, including hidden ones:

```bash
cd inhere
ls -la
```

I saw a file named `.hidden` and read it using `cat`:

```bash
cat .hidden
```

The password was right there!

---