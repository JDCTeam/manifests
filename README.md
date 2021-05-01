
```bash
git commit --amend --author "Author <email@address.com>"
```

So it should look like this once you get all of the author's information

```bash
git commit --amend --author "Spencer McGillicuddy <spencer.the.bestest@gmail.com>"
```

Alternatively, adding as part of the original `git commit` message is preferred and done like the following:

```bash
git commit --author="Author <email@address.com>" -m "[commit message]"
```

This saves time, and when part of your normal routine, prevents the infamous "ermahgerd I forgot to add authorship -
let me fix it because I was found out!" message.


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
