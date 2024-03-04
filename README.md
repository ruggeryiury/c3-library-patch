<div align=center>
<img src='./images/rb3logo.webp' width='32px'>
</div>

<div align=center>
<img src='https://img.shields.io/github/last-commit/ruggeryiury/c3-library-patch?color=%23DDD&style=for-the-badge' /> <img src='https://img.shields.io/github/repo-size/ruggeryiury/c3-library-patch?style=for-the-badge' /> <img src='https://img.shields.io/github/issues/ruggeryiury/c3-library-patch?style=for-the-badge' /> <img src='https://img.shields.io/github/package-json/v/ruggeryiury/c3-library-patch?style=for-the-badge' />
</div>

- - - -

__C3 Library Patch__ provides several missing metadata informations (like vocal tonic note, rating), fixes many album art and other discrepancies for many customs from the large C3 catalog to make your song library look more structured and homogenic while playing customs!

C3 Library Patch has metadata updates for __178__ customs (_as on version 1.0.3_)!

## Installation (using Rock Band 3 Deluxe):

- __Clone/Download the *Rock Band 3 Deluxe* repository:__
  -  To install the *C3 Library Patch*, you need to clone the [*Rock Band 3 Deluxe* repository](https://github.com/hmxmilohax/rock-band-3-deluxe) to manually generate a patch file for Rock Band 3.
- __Clone/Download *this* repository:__
  -  If you want to download this repository as a `.zip` file, just go on the repository's main page, click on the blue `<> Code` button on the top, then select `Download ZIP` (or click [here](https://github.com/ruggeryiury/c3-library-patch/archive/refs/heads/main.zip)).
- __Set up *Rock Band 3 Deluxe* to merge all missing metadata information from *C3 Library Patch*:__
  - Once cloned/downloaded the *Rock Band 3 Deluxe* repository, go to `_ark/songs` inside of it and edit the `missing_song_data.dta`, adding this to the end of the file (and saving the file after):
  
    ```plaintext
    #merge ../dx/song_updates/c3_library_patch.dta
    ```
- __Copy the `c3_library_patch.dta` file:__
  - Copy the `c3_library_patch.dta` file from __this__ repository and place it on `_ark/dx/song_updates` folder inside the __*Rock Band 3 Deluxe* repository__ folder you cloned/downloaded.
- __Copy all *C3 Library Patch* files from the `updates` folder to *Rock Band 3 Deluxe*:__
  - Copy all contents from the `updates` folder from __this__ repository to `_ark/songs/updates` folder inside the __*Rock Band 3 Deluxe* repository__ you cloned/downloaded.
- __Build the patch:__
  - Follow the instructions on the [*Rock Band 3 Deluxe* repository](https://github.com/hmxmilohax/rock-band-3-deluxe) to properly build your own version of the *Rock Band 3 Deluxe* patch and place it on your system/emulator.
- __Enjoy *C3 Library Patch*!__

## Frequently Asked Questions

- *The updated metadata is not showing in one/a few customs, but some others do. What's going on?*
  - Probably the charter updated the song itself and changed the shortname of the custom you've downloaded. Contact me if this happens.

- *The metadata of the song is updated but I notice the lipsync/venues is gone. What's going on?*
  - Probably I forgot to properly place the updated song's MILO file inside the patch. All songs that has fixed album arts must have a copy of the MILO file inside the patch (since the patch tries to read both files from the patch and not from the custom file anymore). Contact me if this happens.