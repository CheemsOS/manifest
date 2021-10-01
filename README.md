CheemsOS

### Requirements
Before start to compiling RohieOS for your own device, some requirements as explained bellow:
- 16GB RAM (Swap can be helpful)
- Quadcore Processor
- 150GB Free Disk Space

---------------------------------------------------------------------------------------

To initialize your local repository, use a command like this:

```bash
repo init -u https://github.com/CheemsOS/manifest.git -b 11

```
You can alternatively use this command to save some space and time :

```bash
repo init --depth=1 -u https://github.com/CheemsOS/manifest.git -b 11

```

Then to sync up:

```
repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags
```
You can just use `repo sync` or above command, but this will save you from lot of terminal spam, data and time.
```bash
repo sync -c -q --force-sync --optimized-fetch --no-tags --no-clone-bundle --prune -j$(nproc --all)
```
