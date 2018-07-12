# Our IIIF Images

† Our thanks to Kevin Bowrin, Programmer at Carleton University Library Systems Department, who set up our IIIF server and sent on these details

The images of the manuscript scans for the HIST 4006 course are now available through our new IIIF server.

You can see a list of the images we have stored here:

```text
https://viewer.library.carleton.ca/2018-07-07-hist4006-manuscriptimages/
```

The images are available at URLs like:

```text
https://viewer.library.carleton.ca/2018-07-07-hist4006-manuscriptimages/ARC_manuscript_1_10R.JPG
```

You can see an example of an IIIF client \(OpenSeadragon\) which has been configured to display the .tif files here:

```text
https://viewer.library.carleton.ca/2018-07-07-hist4006-manuscriptimages/view.html
```

The IIIF server URLs for the images look like this:

```text
https://iiif.library.carleton.ca/iiif/2/2018-07-07-hist4006-manuscriptimages%2FARC_manuscript_1_50V%2520%28duo%29.JPG/info.json
https://iiif.library.carleton.ca/iiif/2/2018-07-07-hist4006-manuscriptimages%2FARC_manuscript_1_50V%2520%28duo%29.JPG/full/full/0/default.jpg
```

The IIIF server Image API documentation can be found here:

```text
https://iiif.io/api/image/
```

Our image server is:

```text
https://medusa-project.github.io/cantaloupe/
```

If you have an image available at:

```text
https://viewer.library.carleton.ca/2018-07-07-hist4006-manuscriptimages/ARC_manuscript_1_10R.JPG
```

The IIIF server will serve the image, full region \(the complete image\), full size \(not scaled\), and with 0 rotation at:

```text
https://iiif.library.carleton.ca/iiif/2/2018-07-07-hist4006-manuscriptimages%2FARC_manuscript_1_10R.JPG/full/full/0/default.jpg
```

The IIIF server will serve the image, with a square region, scaled to 100x100 pixels, mirrored with 180 degrees rotation, in grayscale, at:

```text
https://iiif.library.carleton.ca/iiif/2/2018-07-07-hist4006-manuscriptimages%2FARC_manuscript_1_10R.JPG/square/100,100/!180/gray.jpg
```

The IIIF server will provide the image information at:

```text
https://iiif.library.carleton.ca/iiif/2/2018-07-07-hist4006-manuscriptimages%2FARC_manuscript_1_10R.JPG/info.json
```

The image information URL is the URL used by most IIIF clients to ‘point to’ the image. For example, in the openseadragon example I set up, the javascript code looks like:

```text
    var viewer = OpenSeadragon({
        id: "viewer",
        collectionMode:       true,
        collectionRows:       3,
        collectionTileSize:   1024,
        collectionTileMargin: 56,
        prefixUrl: "/openseadragon/openseadragon-bin-2.3.1/images/",
        tileSources: [
            "https://iiif.library.carleton.ca/iiif/2/2018-07-07-hist4006-manuscriptimages%2FARC_ms_11.tif/info.json",
            …
            "https://iiif.library.carleton.ca/iiif/2/2018-07-07-hist4006-manuscriptimages%2FCUAG_1995.62.9a.tif/info.json",
            "https://iiif.library.carleton.ca/iiif/2/2018-07-07-hist4006-manuscriptimages%2FCUAG_1995.62.9b.tif/info.json"
        ]
    });
```

To build the IIIF link:

The “identifier” for the image is everything after

```text
https://viewer.library.carleton.ca/
```

Replace

```text
https://viewer.library.carleton.ca/
```

with

```text
https://iiif.library.carleton.ca/iiif/2/
```

In the identifier, you need to replace the / character with %2F Also in the identifier, you need to replace the sequence of characters %20 with %2520. Finally, you need to add the image request parameters /{region}/{size}/{rotation}/{quality}.{format} or the image information request parameter /info.json to the end of the URL. For example, t he link to the image with filename “ARC\_manuscript\_1\_21V.JPG” is:

```text
https://viewer.library.carleton.ca/2018-07-07-hist4006-manuscriptimages/ARC_manuscript_1_21V.JPG
```

The IIIF image information link would be:

```text
https://iiif.library.carleton.ca/iiif/2/2018-07-07-hist4006-manuscriptimages%2FARC_manuscript_1_21V.JPG/info.json
```

The link to the image with filename “ARC\_manuscript\_1\_16V \(duo\).JPG” is

```text
https://viewer.library.carleton.ca/2018-07-07-hist4006-manuscriptimages/ARC_manuscript_1_16V%20%28duo%29.JPG
```

The IIIF image information link would be:

```text
https://iiif.library.carleton.ca/iiif/2/2018-07-07-hist4006-manuscriptimages%2FARC_manuscript_1_16V%2520%28duo%29.JPG/info.json
```

