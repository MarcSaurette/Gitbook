# Using IIIF Manifests

## What is a Manifest?

We don't need to define what is a manifest because IIIF consortium has already done a great job doing that [here](https://iiif.github.io/training/iiif-5-day-workshop/day-two/5-anatomy-of-a-basic-manifest.html). IIIF is a way to  serve images but it is also a way to communicate information about those images. The **manifest** does that - in part telling viewers how to present the images \(so that fol. 2r comes after fol. 1v.\), but also containing key information about the images. We have been using CUAG fol. 13 as our example, but we won't since, it being post-medieval I never added it to the Omeka site.  So we'll use another, the _Yorkshire Deed by William Bron, Collector of the King’s Rents_ instead_._

If you navigate to our Omeka site, we will find CUAG fol. 13  \(you will need to sign into Omeka\):

```
https://medievalottawa.org/admin/items/show/290
```

If you navigate to the very bottom of the page, you will find the manifest url. [Click on it](https://medievalottawa.org/oa/items/290/manifest.json) and you will see the following. Look for what kinds of information it contains:

```markup
{
"@context": "http://www.shared-canvas.org/ns/context.json",
"@id": "https://medievalottawa.org/oa/items/290/manifest.json",
"@type": "sc:Manifest",
"label": "Carleton University Archives and Research Collections",
"sequences": [
{
"@id": "https://medievalottawa.org/oa/items/290/sequence.json",
"@type": "sc:Sequence",
"label": "",
"canvases": [
{
"@id": "http://82b464c8-82f5-40ad-b08f-c381cfc32972",
"@type": "sc:Canvas",
"label": "Yorkshire Deed by William Bron, Collector of the King’s Rents",
"height": 4495,
"width": 6774,
"images": [
{
"@context": "http://iiif.io/api/presentation/2/context.json",
"@id": "http://37b29be2-519d-4682-8231-7733cb7e76df",
"@type": "oa:Annotation",
"motivation": "sc:painting",
"resource": {
"@id": "https://iiif.library.carleton.ca/iiif/2/2018-07-07-hist4006-manuscriptimages%2FARC_ms_26.tif/full/full/0/default.jpg",
"@type": "dctypes:Image",
"format": "image/jpeg",
"service": {
"@context": "http://iiif.io/api/image/2/context.json",
"@id": "https://iiif.library.carleton.ca/iiif/2/2018-07-07-hist4006-manuscriptimages%2FARC_ms_26.tif",
"profile": [
"http://iiif.io/api/image/2/level2.json",
{
"formats": [
"jpg",
"tif",
"gif",
"png"
],
"maxArea": 400000000,
"qualities": [
"bitonal",
"default",
"gray",
"color"
],
"supports": [
"regionByPx",
"sizeByW",
"sizeByWhListed",
"cors",
"regionSquare",
"sizeByDistortedWh",
"sizeAboveFull",
"canonicalLinkHeader",
"sizeByConfinedWh",
"sizeByPct",
"jsonldMediaType",
"regionByPct",
"rotationArbitrary",
"sizeByH",
"baseUriRedirect",
"rotationBy90s",
"profileLinkHeader",
"sizeByForcedWh",
"sizeByWh",
"mirroring"
]
}
]
},
"height": 4495,
"width": 6774
},
"on": "http://82b464c8-82f5-40ad-b08f-c381cfc32972"
}
],
"description": "This legal document (chirograph) addressed to William Goldale is a judicial summons demanding that the offending parties pay in full the back rents that are owed to the King for their tenancy on his lands. It outlines the consequences of this action and of further inaction.",
"attribution": "Carleton University Archives and Research Collections (CUARC)",
"metadata": [
{
"label": "Subject",
"value": "Deed concerning rent collection from land holdings in Snayth, England on behalf of King Henry V."
},
{
"label": "Creator",
"value": "William Bron"
},
{
"label": "Source",
"value": "http://4800d54a-bd4d-4cbb-9719-515dffa08978<br>Ottawa, Carleton University, Carleton University Archives and Research Collections, Charter 2"
},
{
"label": "Date",
"value": "May 24, 1405"
},
{
"label": "Contributor",
"value": "Brasseur, Kate"
},
{
"label": "Relation",
"value": "Other half of indented parchment: unknown whereabouts"
},
{
"label": "Format",
"value": "IIIF Image<br>Parchment"
},
{
"label": "Language",
"value": "Latin, with intermittent English"
},
{
"label": "Type",
"value": "Charter, Chirograph"
},
{
"label": "Coverage",
"value": "Yorkshire, England"
},
{
"label": "Provenance",
"value": "Previous owners, Bernard Quaritch Ltd of London, referenced this item as D102 (red ink on envelope) and sold the item, along with a handwritten transcription (unknown author), for 8 pounds. "
},
{
"label": "Rights Holder",
"value": "Carleton University, MacOdrum Library, Archives and Research Collections"
}
],
"otherContent": [
{
"@id": "https://medievalottawa.org/oa/items/290/annolist.json",
"@type": "sc:AnnotationList"
}
]
}
]
}
],
"description": "This legal document (chirograph) addressed to William Goldale is a judicial summons demanding that the offending parties pay in full the back rents that are owed to the King for their tenancy on his lands. It outlines the consequences of this action and of further inaction.",
"attribution": "Carleton University Archives and Research Collections (CUARC)",
"metadata": [
{
"label": "Subject",
"value": "Deed concerning rent collection from land holdings in Snayth, England on behalf of King Henry V."
},
{
"label": "Creator",
"value": "William Bron"
},
{
"label": "Source",
"value": "http://4800d54a-bd4d-4cbb-9719-515dffa08978<br>Ottawa, Carleton University, Carleton University Archives and Research Collections, Charter 2"
},
{
"label": "Date",
"value": "May 24, 1405"
},
{
"label": "Contributor",
"value": "Brasseur, Kate"
},
{
"label": "Relation",
"value": "Other half of indented parchment: unknown whereabouts"
},
{
"label": "Format",
"value": "IIIF Image<br>Parchment"
},
{
"label": "Language",
"value": "Latin, with intermittent English"
},
{
"label": "Type",
"value": "Charter, Chirograph"
},
{
"label": "Coverage",
"value": "Yorkshire, England"
},
{
"label": "Provenance",
"value": "Previous owners, Bernard Quaritch Ltd of London, referenced this item as D102 (red ink on envelope) and sold the item, along with a handwritten transcription (unknown author), for 8 pounds. "
},
{
"label": "Rights Holder",
"value": "Carleton University, MacOdrum Library, Archives and Research Collections"
}
],
"service": [
{
"@context": "http://iiif.io/api/search/1/context.json",
"@id": "https://medievalottawa.org/oa/items/290/search",
"label": "Search this manifest with Omeka",
"profile": "http://iiif.io/api/search/1/search"
}
]
}
```

You'll notice the manifest contains a lot of metadata \(in fact all the metadata we have supplied to Omeka\), but also contains links to the images it serves. On line 25 you'll notice this point of information - pointing to the IIIF image server:

```markup
"@id": "https://iiif.library.carleton.ca/iiif/2/2018-07-07-hist4006-manuscriptimages%2FARC_ms_26.tif/full/full/0/default.jpg",
```

Now, let's talk a look at what a big institution does with their manifests. If you take a look at one of the manuscripts at the British Library, we see the manifest looks similar but has a lot more information. We can see the manuscript through the Gallica-run viewer for [_British Library Cotton MS Titus A XXVII_](https://manuscrits-france-angleterre.org/view3if/pl/ark:/81055/vdc_100064372960.0x000001/f8)_._ If you look at the viewer showing the manuscript image it should be familiar - it is the Project Mirador viewer that Omeka also uses. 

If you navigate to the top right corner and click on the i \(info\) icon, a column opens up. At the very bottom \(scroll down\) is the IIIF Manifest. Click on [it](https://api.bl.uk/metadata/iiif/ark:/81055/vdc_100064372960.0x000001/manifest.json) and it will take you to the manifest .json file. I won't copy it below, but you will notice that it is HUGE. In part this is because it is a whole manuscript and so it must list every image it wants to share \(while our manifest above has one image on the canvas, this one has hundreds\). It has some basic metadata to describe the manuscript. A complete manuscript description for this ms. can be found [here](http://searcharchives.bl.uk/primo_library/libweb/action/dlDisplay.do?docId=IAMS040-001103518&fn=permalink&vid=IAMS_VU2). 

You will notice that contained in the manifest is some descriptive metadata and also the urls of the images served via IIIF. In the midst of the code, inside the canvas divisions of the .json file we will see the following:

```markup
images": [
{
"@type": "oa:Annotation",
"motivation": "sc:painting",
"resource": {
"@id": "https://api.bl.uk/image/iiif/ark:/81055/vdc_100064507675.0x00000b/full/max/0/default.jpg",
"@type": "dctypes:Image",
"format": "image/jpg",
"service": {
"@context": "http://iiif.io/api/image/2/context.json",
"@id": "https://api.bl.uk/image/iiif/ark:/81055/vdc_100064507675.0x00000b",
"protocol": "http://iiif.io/api/image",
"width": 4529,
"height": 6027,
"tiles": [
....
```

On line 6 you will see a url for one of the first folios. If you copy and paste it into your browser, you will download the image to your computer. 

### Side-by-Side Comparisons

If you wanted to compare two manuscripts side by side you can use Mirador to do that. It is useful for comparing palaeography of your manuscript against another \(with a dated and identified hand\), or comparing different manuscripts of the same text. 

Return to the [Gallica site](https://manuscrits-france-angleterre.org/view3if/pl/ark:/81055/vdc_100064372960.0x000001/f8) and again in the upper right corner locate "Change Layout". Click on it and select a 1x2 grid. You will now have an empty window with a big **+ sign** in the middle. Click on it. 

In the upper right hand corner you will see a box prefaced by the text, "Add new object from URL:". In this box copy the url of the manifest of the charter at Carleton. 

[`https://medievalottawa.org/oa/items/290/manifest.json`](https://medievalottawa.org/oa/items/290/manifest.json)\`\`

You will be brought back to a screen with the British Library manuscript and on the right side should be a copy of the charter at Carleton. Then you can do what you want with the images....

{% hint style="warning" %}
Because the Mirador viewer is accessing large image files it may take up to a minute for the image to load for comparison. 
{% endhint %}

