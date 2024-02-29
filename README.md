<div align=center>
<img src='./images/rb3logo.webp' width='32px'>
</div>

<div align=center>
<img src='https://img.shields.io/github/last-commit/ruggeryiury/c3-library-patch?color=%23DDD&style=for-the-badge' /> <img src='https://img.shields.io/github/repo-size/ruggeryiury/c3-library-patch?style=for-the-badge' /> <img src='https://img.shields.io/github/issues/ruggeryiury/c3-library-patch?style=for-the-badge' /> <img src='https://img.shields.io/github/package-json/v/ruggeryiury/c3-library-patch?style=for-the-badge' /> <img src='https://img.shields.io/github/license/ruggeryiury/c3-library-patch?style=for-the-badge' />
</div>

- - - -

C3 Library Patch provides several missing metadata (like vocal tonic note, rating), fixes many album art and other discrepancies for many customs from the large C3 catalog to make your song library look more structured and homogenic while playing customs!

## Installation (using Rock Band 3 Deluxe):

- __Clone the Rock Band 3 Deluxe repo:__
  -  To install the C3 Library Patch, you need to clone the [Rock Band 3 Deluxe repository](https://github.com/hmxmilohax/rock-band-3-deluxe) to manually generate a patch file for Rock Band 3.
- __Merge all missing metadata information:__
  - Once cloned the Rock Band 3 Deluxe repository, go to `_ark/songs` inside of it and edit the `missing_song_data.dta`, adding `#merge ../dx/song_updates/c3_library_patch.dta` to the end of the file.
- __Copy the `c3_library_patch.dta` file:__
  - Copy the `c3_library_patch.dta` file from this repository and place it on `_ark/dx/song_updates` folder inside the Rock Band 3 Deluxe repository folder you've cloned.
- __Copy all song update files to Rock Band 3 Deluxe:__
  - Copy all contents from the `updates` folder from this repository to `_ark/songs/updates` folder inside the Rock Band 3 Deluxe repository you've cloned.
- __Build the patch:__
  - Follow the instructions on the [Rock Band 3 Deluxe repository](https://github.com/hmxmilohax/rock-band-3-deluxe) to properly build your own version of the Rock Band 3 Deluxe patch.