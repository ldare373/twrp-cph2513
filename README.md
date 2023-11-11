# TWRP CPH2513
## Under Development
This port is currently under development and does not work.
## Compilation
First, download the minimal TWRP android-12.1 tree.

`repo init -u https://github.com/minimal-manifest-twrp/platform_manifest_twrp_aosp.git -b twrp-12.1`

Next, create `.repo/local_manifests/cph2513.xml` and add the following:
```
<?xml version="1.0" encoding="UTF-8"?>
<manifest>
    <remote name="lda" 
        fetch="https://github.com/ldare373"
        pushurl="git@github.com:ldare373"/>
    <project path="device/oplus/cph2513" 
        name="twrp-cph2513"
        remote="lda"
        revision="main"/>
</manifest>
```
You can now sync the source.

`repo sync`
