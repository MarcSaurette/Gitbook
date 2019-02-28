# Look at a TEI folio description

#### Examples of TEI encoded Folio

* Antiphonary folio located at the Beinecke Rare Book and Manuscript Library, catalogued on the [_Fragmentarium_ website](https://fragmentarium.ms/description/F-5xax/383). 
* [TEI xml](https://fragmentarium.ms/description/export/383/F-5xax-383.xml) sheet for the above Antiphonary folio. 

#### Understanding TEI exercise

1. For today's exercise follow the link to [_Fragmentarium_](https://fragmentarium.ms/description/F-5xax/383) __and download the TEI file for the manuscript fragment by pressing the "Download TEI Xml" tab. 
2. Locate the file on your desktop and open with Atom. 
3. Toggle "Soft Wrap" under the "View" menu option to make sure you can see all the text on your screen \(i.e. to avoid really long lines of text scrolling to the right\). 
4. The file defines what version of XML \(line 1\) and TEI  \(line 2\) it is using and what particular standards it is applying. You will notice that the standards link back to version of TEI set up by _Fragmentarium_ on the TEI standards page. 
5. From lines 3-76, you have the TEI header. From lines 77-81, you have the TEI text. Think of this as a sort of header = metadata about the folio, and the text block \(here empty\) as the transcription. 
6. The majority of the TEI header is taken up by the "File Description" `<fileDesc>` that contains several subheadings:
   1. **Title** \(line 6\)
   2. **Edition** \(line 9\)
   3. **Publication** Statement \(lines 11-18\)
      1. Publisher
      2. Availability
      3. Licence
   4. **Source Description** \(lines 19-74\)
      1. ms description \(line 20...\)
         1. _Manuscript identifier_ \(ie shelfmark by location and repository\)
         2. _Head_ \(i.e. title of work by genre, as well as original date and location – here left blank\)
         3. _Physical Description_ here is again mostly left blank but indicates the possibilities of information you could input. 

{% code-tabs %}
{% code-tabs-item title="F-5xax-383.xml" %}
```text
          <physDesc>
            <objectDesc form="Fragment">
              <supportDesc>
                <support>
                  <material/>
                </support>
                <extent>
                  <dimensions type="leaf_orig"/>
                  <dimensions type="written_orig">
                    <width min="168" max="170">168 170</width>
                    <height min="270" max="271">270 271</height>
                  </dimensions>
                  <measure type="pageDimensions">Front pastedown has had ~30mm trimmed unevenly from bottom margin</measure>
                </extent>
              </supportDesc>
              <layoutDesc>
                <layout>
                  <dimensions type="line">
                    <height min="5" max="6">5 6</height>
                  </dimensions>
                </layout>
              </layoutDesc>
            </objectDesc>
            <decoDesc>
              <decoNote>The recto of the back pastedown features a 5-line initial P in red penwork filled with yellow (now faded), inhabited with vine motif on blue ground.&#13;
Rubricated initials. <persName/></decoNote>
            </decoDesc>
          </physDesc>
```
{% endcode-tabs-item %}
{% endcode-tabs %}

As you can see if you compare this to the [image](https://fragmentarium.ms/view/page/F-5xax), the description here is minimal - no discussion of music notation, palaeography etc. There is a lot that could be added, but the idea of _Fragmentarium_ in this case is to offer a limited description that has already been established \(taken largely from the reference book noted in line 68, "Hebbard, 2017"\). 

