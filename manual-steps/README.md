# Manual process for updating Oracle Linux

Move existing repo out if the way
```
cd /etc/yum.repos.d
mv public-yum-ol6.repo public-yum-ol6.repo.old
```
(I needed to set proxy variables http_proxy, https_proxy)

Download latest repo ?
```
wget http://public-yum.oracle.com/public-yum-ol6.repo
```

check ol6_latest is "enabled=1"

Optional
```
yum repolist  
```

Update
```
yum update -y
```

Ref
---
https://blogs.oracle.com/wim/entry/setting_up_oracle_linux_6
