# EB-Ketab

EB-Ketab is a modified and improved version of a popular font digitized by Naser Ebrahimi called N-Ketab.

## About the original typeface

The original designer of the typeface in the print, i.e. the letterpress version, that was the inspiration for the font is not known to me. I am not sure if Naser Ebrahimi knew the type designer either. People in the publishing industry probably have a good idea where the typeface originated from and who carved the original typeface for letterpress printing that was in use in Iran for many years and in many publications.

## About N-Ketab, the historic font

So far as I’ve learned, the first attempt to digitize the typeface was done in year 2001 (if you look at the copyright notice inside N-Ketab). Nothing else is known about the artist nor the time or place of creation for N-Ketab. Naser Ebrahimi made other similar-looking fonts at around the same time, all of which are freely available on various websites.

I wished I could find the artist and ask him a few questions about the font, the tool(s) he used to make the font, and the challenges he faced during his digitization of the typeface (if indeed he was the one who first digitized the typeface). I also wished we could ask him about the license he thought he wanted to release his font under. Alas, I haven’t been able to find any trace of him online whatsoever. If you know him, know where I can find him, or know about his destiny, please let me know.

## About EB-Ketab, the improved version

I was translating an ancient text into the Persian language and wanted to use a typeface that was giving the same sense of time, being old, being antique, being from far past, and not modern in any way. I tried many typefaces with various successes. Most typefaces I found on the Internet were either way too modern looking, incomplete, or way too familiar looking, neither of which were desirable character traits for my project. I found myself coming back to N-Ketab over and over.

However, there were serious shortcomings with N-Ketab. I found two broad categories of problems with the original font: (1) No proper kerning and (2) no proper positioning of the diacritics.

The problem was that none of the glyphs had any anchors to determine where the marks on top or at the bottom should have been placed. As a result, the word-processor’s typesetting engine would have decided as to where to place those marks. And the result would have been useless. The word-processors, when they cannot find a proper anchor placement for a mark, will add the mark on top or the bottom of a glyph and push it to the highest or the lowest limits possible, so to stay on the safe side and not to cause unintended collisions between the diacritics and other marks or glyphs. That looks horrible when applied to a Persian script. Every mark will look out of place, either way higher or way too lower than they should have been. Also, when there is no kerning information for a given pair, the word-processor merely uses the right and the left bearings of the letterbox to typeset the characters. The result of this behaviour also would be very unpleasant with any Persian script.

The way to fix those two problems seemed to be beyond my technical knowledge and ability, so I tried to find the original artist. When I failed to find him, I tried to find other artists who released similar fonts, variations of N-Ketab, to see if there were anyone who could help fix the font. I did not know how much work was needed to fix the kerning and the positioning of the marks.

I found a gentleman who worked on a re-release of the same font a few years ago and contacted him. Although we exchanged a few words, it didn’t go that far. So, I ran out of most options. The last resort was to try to fix the issue by myself.

To approach the task, I needed a font editor, and the only one I could get my hands on without paying a lot was FontForge. There were other free and open-source candidate available, but all were either extremely limited in features, or not ready for any serious work. So, I started to use FontForge to learn how to fix N-Ketab.

At first, things seemed to be straightforward: I would open a glyph, add the missing anchors, adjust the kerning pairs (which did not exist. Oops!), and I would be finished. However, things did not pan out as I expected.

FontForge is a great software for a beginner who cannot spend a dime on anything, let alone on a piece of software, but still wants to try their hand at font design. On paper, it has almost everything you might ever want. In practice, it is unstable, clunky, with a horrible GUI that results in a poor user experience, filled with hundreds of bugs, that constantly crashes and burns all your hard work up into smokes. No amount of Crtl+S will save you since the software has various bugs just for that too up its sleeves, which you will learn about only *after* several catastrophic crashes.

After spending a couple of weeks and countless hours on FontForge, I felt that I made almost no progress. So, I decided to look into the commercial, alternative font editors. Some of them were priced so high that there were no chance I could ever buy a license for. One, however, came on top. The features, the price, the GUI, and the user experience looked very promising (used the trial version to evaluate its value for my project). Eventually I gambled and bought the full, commercial license for that software. It is called FontCreator. So, EB-Ketab was constructed from bottom-up inside of FontCreator. Once you use a proper, professional software, however painful the license fee might have been, you cannot look back, since the abilities and features of them are far more superior than many freely available alternatives (that is not *always* the case though).

FontCreator allowed me to see the font in a different light. I could see new possibilities, things that I couldn’t see in other font editors. I could see what was related to what, how the kerning was done (or not done in this case), how to adjust the positioning of the marks and other elements, substitutions, etc. So, the initially impossible task of fixing the font looked a lot more tractable.

After spending several more weeks on the font inside FontCreator, the resulting font was way too different than the original font and needed a new name. I assumed ‘N-Ketab’ as a reserved font name, however I did not find any evidence to that effect. Since EB-Ketab was vastly different from N-Ketab, it won’t have been right to install it over N-Ketab. EB-Ketab is almost a different font, so I gave it a new reserved font name of EB-Ketab to differentiate it from N-Ketab and to avoid installing it over N-Ketab by accident. That is how EB-Ketab was born.

To have a sound skeleton for EB-Ketab, I did NOT use N-Ketab font, since it lacked kerning and a whole lot of other things. I started from a typical, standard Persian font, receated the glyphs based on N-Ketab in the new home, and then deleted the unused glyphs and characters in the destination. This way, the originally-defined kerning pairs were preserved. So, I had something to start from and to work on. After trimming down the resulted font and removing all the unnecessary characters, glyphs, or marks, I was left with a relatively clean and workable font.

However, since the kerning settings of the base font was for a different kind of typeface, almost all the kerning settings, all the positioning of the anchors for marks, and the side bearings had to be readjusted to suite EB-Ketab. There were hundreds of kerning pairs that were missing that needed to be added either as individual pairs or classes of characters. But there were only two classes defined in the base font, which were not enough to cover all the possible cases. Therefore, I had to create several new character classes to be used in kerning of paired classes. The rest is history (see the changelog for version 1.0.0 – Initial release).

## Copyright

Copyright © 2022, Eric Bright (<https://sophy.ca/>), with Reserved Font Name EB-Ketab.

This font is based on N-Ketab by Naser Ebrahimi who holds the copyright to the original font (not the typeface).

N-Ketab apparently was released in 2001 and was modified for the next several years. Several other copies of the same font were released by other people, none of which changed anything with the original font, but merely removed and replaced the original copyright notice, author, and designer’s names with their own names and copyright notices. Most, if not all, of those latter copycats could not possibly hold any valid copyright claim over the design of this font.

Naser Ebrahimi seemed to have released another font in the same family called A-Ketab at around the same time, year 2001, and with a copyright year of 2009. It is not clear what the difference(s) between N-Ketab and A-Ketab might be since a close inspection of the fonts did not reveal any visible difference.

The vendor’s URL for N-Ketab is still active, but the vendor(s) do not know anything about Naser Ebrahimi more than the fact that he digitized several old, print typefaces like Rooznameh, Ketab, and other fonts. The vendor explains a font called Rooznameh this way (the emphasis is mine): “Creative graphic designers and creators can use this beautiful font in their works. The font was designed *apparently* designed by a person named Naser Ebrahimi, based on old, print typefaces. Mr. Mojtaba Kimia gave this to us.” This clearly shows that the original author was not known to the vendor any more.

As such, I am going to assume that this font is in public domain unless otherwise is proven.

## License

Copyright © 2022, Eric Bright (<https://sophy.ca/>), with Reserved Font Name EB-Ketab.

This Font Software is licensed under the SIL Open Font License, Version 1.1. This license is included in the repository as a file called LICENSE, and is also available with a FAQ at:
<http://scripts.sil.org/OFL>
