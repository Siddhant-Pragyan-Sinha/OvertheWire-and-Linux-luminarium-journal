## **Level 8 → Level 9**

### **Goal**: Find the only line of text that occurs once in a file.

This level required me to find a unique line in `data.txt`. I used `sort` and `uniq -u`:

```bash
sort data.txt | uniq -u
```

The password was the unique line!

---