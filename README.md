Getting Started
======

To get started with OMNI sources to build TWRP, you'll need to get
familiar with [Git and Repo](https://source.android.com/source/using-repo.html).

To initialize your local repository using the OMNIROM trees to build TWRP, use a command like this:
```bash
    repo init -u git://github.com/JDCTeam/manifests.git -b pitchblack-jf
```

Then to build:
```bash
     cd <source-dir>
     export ALLOW_MISSING_DEPENDENCIES=true
     . build/envsetup.sh
     lunch omni_<device>-eng
     mka recoveryimage
```
