
---

### 4️⃣ `Troubleshooting.md`

```markdown
# Troubleshooting Hard/Soft Link Issues

## 1. Broken Soft Link
```bash
ls -l /tmp/file1_soft
# file1_soft -> /tmp/file1 (No such file or directory)

Fix by recreating the symlink:

ln -sf /tmp/file1 /tmp/file1_soft


