
---

### 3️⃣ `Real-time_Scenarios.md`

```markdown
# Real-time Scenarios: Hard vs Soft Links

### Scenario 1: Software Version Management (Tomcat)
- Application runs in `/opt/tomcat` pointing to Tomcat 9.  
- New version Tomcat 10 is installed in `/opt/tomcat10`.  
- Instead of changing all config files, update symlink:

# Backup old link
```bash
mv /opt/tomcat /opt/tomcat_old
```

# Point to new version
```bash
ln -s /opt/tomcat10 /opt/tomcat
```

