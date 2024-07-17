<div align=center>
<img src='./images/rb3logo.webp' width='32px'>
</div>

<div align=center>
<img src='https://img.shields.io/github/last-commit/ruggeryiury/c3-library-patch?color=%23DDD&style=for-the-badge' /> <img src='https://img.shields.io/github/repo-size/ruggeryiury/c3-library-patch?style=for-the-badge' /> <img src='https://img.shields.io/github/issues/ruggeryiury/c3-library-patch?style=for-the-badge' /> <img src='https://img.shields.io/github/package-json/v/ruggeryiury/c3-library-patch?style=for-the-badge' />
</div>

- - - -

__C3 Library Patch__ provides several missing metadata informations (like vocal tonic note, rating), fixes many album art and other discrepancies for many customs from the large C3 catalog to make your song library look more structured and homogenic while playing customs!

C3 Library Patch has metadata updates for __248__ customs (_as on version 1.0.7_)!

- - - -

## 💠 Table of Contents

- [Installation (using Rock Band 3 Deluxe)](#installation-using-rock-band-3-deluxe)
- [Troubleshooting](#troubleshooting)

# Installation (using Rock Band 3 Deluxe)

- __Clone/Download the *Rock Band 3 Deluxe* repository:__
  -  To install the *C3 Library Patch*, you need to clone the [*Rock Band 3 Deluxe* repository](https://github.com/hmxmilohax/rock-band-3-deluxe) to manually generate a patch file for Rock Band 3.
  -  **NOTE: C3 Library Patch only works properly on [version 1.1.0-beta11](https://github.com/hmxmilohax/rock-band-3-deluxe/releases/tag/v1.1.0-beta11) or newer. Older versions won't load lipsync and venues, but the metadata will work just fine.**
- __Clone/Download *this* repository:__
  -  If you want to download this repository as a `.zip` file, just go on the repository's main page, click on the blue `<> Code` button on the top, then select `Download ZIP` (or click [here](https://github.com/ruggeryiury/c3-library-patch/archive/refs/heads/main.zip)).
- __Set up *Rock Band 3 Deluxe* to merge all missing metadata information from *C3 Library Patch*:__
  - Once cloned/downloaded the *Rock Band 3 Deluxe* repository, go to `_ark/songs` inside of it and edit the `missing_song_data.dta`, adding this to the end of the file (and saving the file after):
  
    ```text
    #merge ../dx/song_updates/c3_library_patch.dta
    ```
- __Copy the `c3_library_patch.dta` file:__
  - Copy the `c3_library_patch.dta` file from __this__ repository and place it on `_ark/dx/song_updates` folder inside the __*Rock Band 3 Deluxe* repository__ folder you cloned/downloaded.
- __Copy all *C3 Library Patch* files from the `updates` folder to *Rock Band 3 Deluxe*:__
  - Copy all contents from the `updates` folder from __this__ repository to `_ark/songs/updates` folder inside the __*Rock Band 3 Deluxe* repository__ you cloned/downloaded.
- __Build the patch:__
  - Follow the instructions on the [*Rock Band 3 Deluxe* repository](https://github.com/hmxmilohax/rock-band-3-deluxe) to properly build your own version of the *Rock Band 3 Deluxe* patch and place it on your system/emulator.
- __Enjoy *C3 Library Patch*!__

# Troubleshooting

- **The updated metadata is not showing in one/a few customs, but some others do:**
  - Probably the charter updated the song itself and changed the shortname of the custom you've downloaded. Contact me if this happens.

- **The metadata of the song is updated but I notice the lipsync/venues is gone:**
  - ~~Probably I forgot to properly place the updated song's MILO file inside the patch. All songs that has fixed album arts must have a copy of the MILO file inside the patch (since the patch tries to read both files from the patch and not from the custom file anymore). Contact me if this happens.~~
    - ***Update:*** *As I mentioned eariler, this behavior has changed as from Rock Band 3 Deluxe `version 1.1.0-beta11`, where album artworks can be read directly from the patch without needing to use the `alternate_path` value on the DTA, and with this, there's no need to have a copy of the song's MILO file on the patch, making this error unlikely to happen on the `version 1.1.0-beta11` or newer.*

- **After installing _C3 Library Patch_, some official songs/DLCs are using artworks from another song:**
  - This happens because a custom is using the same internal shortname of a official song/DLC. Contact me if this happens, as the updated song must be removed from the patch until the charter itself changes the internal shortname of its own custom.