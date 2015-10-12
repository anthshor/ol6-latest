### Pre-Requirement 
 - Install packer

### Install Linux

cloned Stage from original ol6 packer build:

```
git clone https://github.com/shortcutsh/packer-oraclelinux
cp Stage3/* .
```

```
packer build packer_ol6.json
```

root password is Welcome1

## To Do
Add latest patches to build
```
yum update
```
