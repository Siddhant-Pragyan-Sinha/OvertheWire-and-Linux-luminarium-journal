## **Level 2 → Level 3**

### **Goal**: Read a file with spaces in its name.

This level had a file named `spaces in this filename`. At first, I tried `cat spaces in this filename`, but it didn't work because the spaces confused the terminal. I realized I needed to either use quotes or escape the spaces:

```bash
cat "spaces in this filename"
```

or

```bash
cat spaces\ in\ this\ filename
```

Both worked, and I got the password for the next level.

---