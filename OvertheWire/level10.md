## **Level 9 → Level 10**

### **Goal**: Find a string preceded by several `=` characters.

This level had a binary file with some readable text. I used `strings` to extract the text and `grep` to find the password:

```bash
strings data.txt | grep ===
```

The password was right there!

---