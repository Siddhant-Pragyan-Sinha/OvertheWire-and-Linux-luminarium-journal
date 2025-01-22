## **Level 11 → Level 12**

### **Goal**: Decode a ROT13-encoded file.

This level had a file encoded in ROT13. I used the `tr` command to decode it:

```bash
cat data.txt | tr 'A-Za-z' 'N-ZA-Mn-za-m'
```

The password was right there!

---