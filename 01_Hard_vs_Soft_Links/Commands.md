# Hard and Soft Link Commands

### Hard Link
```bash
# Hands-on Commands: Hard vs Soft Links

## 1. Hard Link
```bash
# Create a file
echo "Hello L3 Engineer" > /tmp/file1

# Create a hard link
ln /tmp/file1 /tmp/file1_hard

# Verify
ls -li /tmp/file1 /tmp/file1_hard

2. Soft Link

# Create a soft link
ln -s /tmp/file1 /tmp/file1_soft

# Verify
ls -li /tmp/file1 /tmp/file1_soft


Soft link has a different inode number.

It points to the filename /tmp/file1.

3. Test Behavior

# Delete original file
rm /tmp/file1

# Check links
cat /tmp/file1_hard   # Works
cat /tmp/file1_soft   # Broken link





