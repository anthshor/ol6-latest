### Pre-Requirement 
 - Install packer

### Install Linux

cloned Stage from original ol6 packer build:

```
git clone https://github.com/shortcutsh/packer-oraclelinux
cp Stage3/* .
```

To package box file locally
```
packer build ol66.json | tee packer-build-ol66.log
```

root password is Welcome1


