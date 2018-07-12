# Installing Medieval Unicode

Our word _alphabet_ comes from the names of the first two letters of the Greek alphabet \(alpha + beta\). In Latin, the alphabet was called an _abecedarium_ \(A, Be, Ce, D -arium\) from the names of the first four letters in the Latin alphabet. Transcribing needs so much more than Modern English's twenty-six letters, however.

Transcribing by hand means that once you have deciphered the text you can reproduce easily and quickly what you see on the page. A digital transcription that retains the characters/ glyphs of the original text, however, is more difficult, as you will need to use a special characters atypical in modern usage. Two decades ago, there was not an option to use non-standard Latin characters on your computer, but in the past decade we have seen considerable advances in establishing standards for a wider range of characters \(in the Latin alphabet, but also in Runic and non-Western alphabets\). We will access these characters in [**unicode**](https://en.wikipedia.org/wiki/Unicode_input). We can thank a small group of dedicated scholars who founded the Medieval Unicode Font Initiative \([MUFI](https://folk.uib.no/hnooh/mufi/)\), which has set out to make a diverse range of manuscript characters reproducible digitally.

Setting up your computer to use unicode and have access to historical fonts takes a few steps, but is straightforward. To use unicode for medieval scripts, however, is a bit more arcane; you might feel like you're a codebreaker trying to crack the Enigma device. As part of this process, we'll put together a list of the most typical characters you'll use in transcribing your folios.

To use medieval characters in your transcriptions, download the two MUFI codebooks organized by [letters](http://bora.uib.no/bitstream/handle/1956/10699/MUFI-Alphabetic-4-0.pdf) and other symbols and [characters](http://bora.uib.no/bitstream/handle/1956/10699/MUFI-CodeChart-4-0.pdf). Like Capelli's guide to medieval abbreviations, these allow you to choose specific characters to match what you see on the page. Before you can use them, however, you will need to get set up to use unicode.

## Setting up Unicode to run on your machine.

1. Set up your device to use unicode. On my Mac, I first enabled Unicode Hex Input in System Preferences -&gt; Keyboard -&gt; Input Sources \(more detailed [instructions here](https://poynton.ca/notes/misc/mac-unicode-hex-input.html)\). The wikipedia article on [unicode](https://en.wikipedia.org/wiki/Unicode_input) outlines how to enable unicode on different platforms.
2. Download a font that will allow you to use medieval unicode features \(a much wider base of characters than one normally uses\) from [options](https://folk.uib.no/hnooh/mufi/fonts/index.html) suggested by MUFI.  I would suggest you download and install the [Andron](https://folk.uib.no/hnooh/mufi/fonts/Andron/AND_SCR_WEB_3.0.zip) font, but [Junicode](http://junicode.sourceforge.net/) and [Titus](http://titus.fkidg1.uni-frankfurt.de/unicode/tituut.asp) also work well.
3. It should be as easy as double clicking on the file\(s\) to add them to a Mac or Windows computer. If you are using Linux, in takes a few more [steps](https://askubuntu.com/questions/3697/how-do-i-install-fonts).
4. Open up a word processor and after selecting the font you have installed, attempt to type some medieval characters, many of which can't be reproduced in markdown \(and thus can't be shown here\).
5. With the option key held down, type EEC5. This should input a small ligature ct \(i.e. a c and t together linked by a little curvy pen flourish\).
6. You should see something that looks like "đ" \(a small letter d with cross stroke\), if you hold down the option key and type "0111".
7. Looking through the two MUFI code books you have downloaded, look for and try out other characters. Not all characters will be the same as indicated in the codebook \(some fonts like Junicode, were completed before the most recent standards were set\).

## Working with MUFI Unicode

1. By this class, you should already have completed a handwritten transcription of your folio. Your goal now is to write it out as an abbreviated text using the now available \(to you\) unicode characters. Go!
2. Post the completed file in your personal Github repository as a pdf, named "LastName-MsX-UnicodeTranscription" \(where LastName is replaced by your last name, and X \[of MsX\] is replaced the number of your folio\).

