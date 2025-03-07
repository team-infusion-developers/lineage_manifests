# Lineage Manifests
Build Lineage 16.0 for i9515 (ALPHA)

![lineage logo](https://github.com/linusdan/local_manifests/raw/lineage-16.0/lineage.png)


```
1. mkdir -p lineage-16.0

2. cd lineage-16.0

3. Initialize your local repository using the Lineage trees, use a command
  repo init  --depth=1 -u git://github.com/LineageOS/android.git -b lineage-16.0
  
4. Sync it:
   repo sync

5. Clone my repo:
  git clone https://github.com/team-infusion-developers/lineage_manifests.git -b lineage-16.0 .repo/local_manifests

6. Sync the repo:
  repo sync --no-tags --no-clone-bundle --force-sync -c

7. Add vendorsetup.sh in device/samsung/jfvelte:
 cd device/samsung/jfvelte && wget -c https://raw.githubusercontent.com/team-infusion-developers/lineage_manifests/lineage-16.0/vendorsetup.sh && cd ../../..

8. To build:
  . build/envsetup.sh
  lunch jfvelte
  brunch jfvelte
```


Credits
-------
* [**rINanDO**](https://github.com/rINanDO)
* [**LineageOS**](https://github.com/LineageOS)
