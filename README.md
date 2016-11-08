# National Geographic daily background

Change your background everyday with national geographic photography.

To install it:
- place `natgeo` script into `/etc/network/if-up.d/` to execute the script when internet connection is up,
- set your custom uri in the script,
- (re)connect your pc to internet,
- set the img downloaded as your background.

You can create a history by uncommenting this line:
```bash
cp $image_uri $history_folder$(date +%d-%m-%Y).jpg
```

Dependency:
- curl (get url of photo)
- wget (download photo)
- jq   (parse json)
