Atiga Devices Manifests
=======================

Getting Started
---------------

To get started with LineageOS-Next, you'll need to get familiar with [Source Control Tools](https://source.android.com/setup/develop).

To initialize your local repository using the LineageOS trees, use a command like this:
```bash
repo init --depth=1 -u https://github.com/LineageOS-Next/next.git -b next-1.0 --git-lfs
```

Clone this repository in `.repo/local_manifests`:
```bash
git clone --single-branch -b next-1.0 https://github.com/Atiga-Stuff/atiga_local_manifests.git .repo/local_manifests
```

Then to sync up:
```bash
repo sync -c --no-clone-bundle --no-tags --optimized-fetch --prune --force-sync -j8
```
