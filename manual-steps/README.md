### Manual process for updating Oracle Linux

Move existing repo out if the way
```
cd /etc/yum.repos.d
mv public-yum-ol6.repo public-yum-ol6.repo.old
```

Set proxy variables http_proxy, https_proxy if required

Download latest repo
```
wget http://public-yum.oracle.com/public-yum-ol6.repo
```

Check ol6_latest is "enabled=1"

Optional step
```
yum repolist  
```

Update
```
yum update -y
```

###Reference
https://blogs.oracle.com/wim/entry/setting_up_oracle_linux_6
