# Ansible Role - yoshihisa:ixgbevf

This Ansible role provides a Intel ixgbevf driver for SR-IOV using DKMS.

# Usage

In this example we configutation AWS EC2 and version 4.5.3.

```
---
- hosts: m4.large
  roles:
    - {role: yoshihisa:ixgbevf, ixgbevf_version: 4.5.3, ixgbevf_tar_sha1_hash: 8ef708a0d5d640405a50b6fa6a924800441b2d4c}
```

You put archive file in `files`.The archive file name should be `ixgbevf-4.5.3.tar.gz`.   
You can find from [SourceForge](https://sourceforge.net/projects/e1000/files/ixgbevf%20stable/).  
If can not find in `files`, download from SourceForge at runtime.  
This sha1 hash is used to validate the downloaded archive file.  
you configure value from upstream or compute.

# Supprt Platforms

EL6 and 7.

# License

MIT License
