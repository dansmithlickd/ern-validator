# ern validator api

https://github.com/ddexnet/ern-validator-api

# installation

To build and start webserver on port 6060

```
chmod +x start.sh
./build.sh
docker-compose up
```

# useage

curl -X POST -F 'messageSchemaVersionId=ern/341' -F 'messageFile=sme-album.xml' -F 'releaseProfileVersionId=commonreleasetypes/14/AudioAlbumMusicOnly' localhost:6060/api/json/validate

# to do

Build creates zip in target which contains the commonreleasetypes which has been manually copied to root dir this should be
copied on build to root/unzipped in target folder.