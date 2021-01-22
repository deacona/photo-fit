# photo-fit
Organising a shedload of photos

<br />

## Useful stuff

<!-- DESKTOP_PATH=Test/Desktop/
DOCUMENTS_PATH=Test/Documents/
PHOTOS_PATH=Test/Pictures/
EXTERNAL_PATH=Test/External/ -->

```
DESKTOP_PATH=/Users/`whoami`/Desktop/
DOCUMENTS_PATH=/Users/`whoami`/Documents/
PHOTOS_PATH=/Users/`whoami`/Pictures/Photos\ Library.photoslibrary/Masters/
EXTERNAL_PATH=/Volumes/My\ Passport\ for\ Mac/

declare -a FOLDER_LIST=("${DESKTOP_PATH}", "${DOCUMENTS_PATH}", "${PHOTOS_PATH}", "${EXTERNAL_PATH}")

for i in "${FOLDER_LIST[@]}"; do
    dir_count=`find "${i}" -mindepth 1 -type d|wc -l`
    file_count=`find "${i}" -mindepth 1 -type f|wc -l`
    total_size=`du -sm "${i}"`
    echo "${i}","${dir_count}","${file_count}","${total_size}"
done
```

## Phase 1. If I Could Turn Back Time

## Phase 2. Get Off Of My Cloud

## Phase 3. Every Picture Tells A Story
