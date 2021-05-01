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
     export ALLOW_MISSING_DEPENDENCIES=true && LC_ALL=C
     . build/envsetup.sh
     lunch omni_jflte-eng
     mka recoveryimage
```
