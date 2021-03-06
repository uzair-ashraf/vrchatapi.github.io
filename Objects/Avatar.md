!>  Special types are listed separately below relevant objects in this file.

# Objects

## Avatar object

Key | Type | Description
----|------|------------
name | string | Name of avatar
description | string | Avatar's description
id | string | Avatar ID (prefixed by 'avtr')
authorName | string | Name of user who created avatar
authorId | string | User ID of user who created avatar (Normally prefixed by 'usr', some exceptions - see 'The Great Pug' author id)
tags | array | Array of user defined tags (max of 5)
version | integer | Upload version of avatar
featured | boolean | If the avatar is featured
created_at | string | Date and time avatar was first uploaded
updated_at | string | Date and time avatar was last uploaded
releaseStatus | [`ReleaseStatus`](Objects/Avatar.md?id=releasestatus) | Release status of avatar
assetUrl | string | Bundled avatar file url (.vrca)
assetVersion | string | Unknown
assetUrlObject | JSONArray | Unknown (Returns empty) - Only returns if you are authenticated and own the avatar
platform | string | Platform avatar was uploaded from
imageUrl | string | Cover image of avatar
thumbnailImageUrl | string | Small cover image of avatar
unityVersion | string | Version of unity avatar was upload from
unityPackageUrl | string | Full unitypackage file that can be used in unity as is (.unitypackage). Looks to be no longer used
unityPackageUrlObject | JSONArray | Unknown (Returns empty)
unityPackages | array | Array of [`unityPackage`](Objects/unityPackage.md?id=unitypackage-object) objects

# Special types

## ReleaseStatus

ReleaseStatus is a string, being one of the following:
 - "public" Everyone can see and use an avatar with this releaseStatus
 - "private" Only owner can see and use an avatar with this releaseStatus
 - "hidden" Avatar has been deleted by its owner, only admin can see an avatar with this releaseStatus
