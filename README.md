# Broken By The Scream Song Sorter

https://bbtssort.github.io/

Want to create your own sorter, see the template at https://github.com/mstie/band-sorter-template

# Customizing this repo

This repo is a copy of the BBTS sorter. You'll need to do the following to customize it to another band:

1. Look through [index.html](./index.html) for all references to BBTS such as links and other text. Replace them with the links for the new band.
2. Replace all the images in [img/albums](./img/albums) with album covers for the new band. See [CONTRIBUTING.md](./.github/CONTRIBUTING.md#image-sizes) for recommended image sizes
3. Replace the [img/bandlogo.png](./img/bandlogo.png) with another image. If it's not a `png` file be sure to update [index.html](./index.html) with the correct name
4. Replace the [img/favicon.png](./img/favicon.png) and [img/apple-touch-icon.png](./img/apple-touch-icon.png) with the favicon from the band's site. This is usually located at `https://<bandwebsite>/favicon.ico`. If it's not there you'll need to find it in the web page's source.
5. Update all the albums and songs in [songlist.js](./js/songlist.js)

# Adding albums and songs

All song data lives in [js/songlist.js](./js/songlist.js). One album is one object in the `RAW_ALBUMS` array.

Follow the steps below to add or modify albums and songs:

1. **Save the cover art**
   * Drop the cover image into [img/albums/](./img/albums). Square aspect ratio is best (the UI crops to 1:1). PNG or JPG both work. Use a short, descriptive filename in camelCase, e.g. `solarStrain.jpg`. See the table in [Image sizes](#image-sizes) below for recommended sizes.
2. **Add a new album or update songs**
    * See [./js/README.md](./js/README.md) for instructions

3. **Test your changes**
   * Run `npm start` to open the web browser to test your changes. Allow Node.js if prompted. If you get an error, try running `npm install` first.

4. **Push your changes to GitHub**
   * No code changes needed elsewhere. Push your changes to GitHub and you're done.
