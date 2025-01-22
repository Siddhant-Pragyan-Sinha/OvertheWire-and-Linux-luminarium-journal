## **Level 4 → Level 5**

### **Goal**: Find the human-readable file in a directory.

This level had a bunch of files in the `inhere` directory, but only one was human-readable. I used the `file` command to check each file:

```bash
file ./-file*
```

I found that `-file07` was labeled as `ASCII text`. I read it using `cat`:

```bash
cat ./-file07
```

And there was the password!

---