# Linux Command Cheat Sheet: Zero to Hero for DevOps & Cloud Engineers

# 1. Navigation

## pwd
Print current directory.

```bash
pwd
```

Example Output:
```bash
/home/kuldeep/projects
```

## ls
List files and folders.

```bash
ls
ls -la
```

Examples:
```bash
ls
ls -lh
```

---

# 2. Directory Management

## mkdir
Create directory.

```bash
mkdir logs
mkdir -p app/logs/archive
```

## rmdir
Remove empty directory.

```bash
rmdir test
```

## rm
Delete files/directories.

```bash
rm file.txt
rm -rf folder
```

Warning:
```bash
rm -rf /
```
Never run.

---

# 3. File Operations

## touch
Create file.

```bash
touch app.log
```

## cp
Copy files.

```bash
cp a.txt b.txt
cp -r source target
```

## mv
Move or rename.

```bash
mv old.txt new.txt
mv file.txt /tmp
```

## cat

```bash
cat file.txt
```

## less

```bash
less app.log
```

## head

```bash
head -10 app.log
```

## tail

```bash
tail -f app.log
```

DevOps Tip:
Follow logs live using:

```bash
tail -f /var/log/nginx/access.log
```

---

# 4. Search

## grep

```bash
grep ERROR app.log
grep -i failed app.log
grep -r nginx .
```

## find

```bash
find . -name "*.js"
find /var -type f
```

## locate

```bash
locate nginx.conf
```

---

# 5. Permissions

## chmod

```bash
chmod 755 script.sh
chmod +x script.sh
```

Meaning:

7 = rwx

5 = r-x

## chown

```bash
chown ubuntu:ubuntu file.txt
```

## ls -l

```bash
ls -l
```

---

# 6. Users

## whoami

```bash
whoami
```

## id

```bash
id
```

## sudo

```bash
sudo apt update
```

## passwd

```bash
passwd
```

---

# 7. Processes

## ps

```bash
ps aux
```

## top

```bash
top
```

## htop

```bash
htop
```

## kill

```bash
kill PID
kill -9 PID
```

## pgrep

```bash
pgrep nginx
```

---

# 8. Networking

## ip

```bash
ip a
ip route
```

## ping

```bash
ping google.com
```

## curl

```bash
curl https://example.com
curl -I https://google.com
```

## wget

```bash
wget https://example.com/file.zip
```

## netstat

```bash
netstat -tulpn
```

## ss

```bash
ss -tulpn
```

## nslookup

```bash
nslookup google.com
```

## dig

```bash
dig google.com
```

## traceroute

```bash
traceroute google.com
```

---

# 9. Disk Management

## df

```bash
df -h
```

## du

```bash
du -sh *
```

## lsblk

```bash
lsblk
```

## mount

```bash
mount
```

---

# 10. Archives

## tar

```bash
tar -cvf backup.tar app/
tar -xvf backup.tar
```

## gzip

```bash
gzip app.log
gunzip app.log.gz
```

## zip

```bash
zip -r app.zip app/
unzip app.zip
```

---

# 11. Package Management

## Ubuntu

```bash
apt update
apt install nginx
apt remove nginx
```

## RHEL/CentOS

```bash
yum install nginx
dnf install nginx
```

---

# 12. Services

## systemctl

```bash
systemctl status nginx
systemctl start nginx
systemctl stop nginx
systemctl restart nginx
systemctl enable nginx
```

---

# 13. SSH

## Connect

```bash
ssh user@server-ip
```

## Copy File

```bash
scp file.txt user@server:/tmp
```

---

# 14. Environment Variables

## View

```bash
env
printenv
```

## Set

```bash
export APP_ENV=prod
```

---

# 15. DevOps Daily Commands

```bash
docker ps
docker logs container
kubectl get pods
kubectl describe pod mypod
kubectl logs mypod
kubectl get nodes
```

---

# 16. Top 20 Interview Commands

```bash
grep
find
awk
sed
tail
head
chmod
chown
ps
top
kill
curl
wget
ssh
scp
tar
df
du
systemctl
journalctl
```

---

# awk Examples

```bash
awk '{print $1}' file.txt
awk '/ERROR/' app.log
```

# sed Examples

```bash
sed 's/dev/prod/g' file.txt
sed -n '1,10p' file.txt
```

---

# journalctl

```bash
journalctl -u nginx
journalctl -f
```

---

# Ultimate DevOps Tips

1. Master grep, find, awk, sed.
2. Use tail -f every day.
3. Learn SSH deeply.
4. Know Linux permissions by heart.
5. Learn networking commands before Kubernetes.
6. Troubleshoot using:
   - ping
   - curl
   - ss
   - systemctl
   - journalctl
7. Be comfortable editing files with vim.
8. Learn bash scripting.
9. Automate repetitive work.
10. Practice on AWS EC2 or a Linux VM daily.

# 30-Day Linux Roadmap

Week 1:
- Files
- Directories
- Permissions

Week 2:
- Processes
- Networking
- Services

Week 3:
- Bash scripting
- Logs
- Monitoring

Week 4:
- Docker
- Kubernetes
- Cloud troubleshooting

