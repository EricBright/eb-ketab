# Changelog

## v1.1.0

* Redesigned the glyph for ae-arab

* Created kerning pairs for the following characters:
  * dal-arab.fina/noon-arab.init
  * waw-arab/space
  * reh-arab.fina/meem-arab.init
  * alef-arab.fina/ain-arab
  * alef-arab.fina/ghain-arab
  * alef-arab.fina/jeem-arab
  * alef-arab.fina/tche-arab
  * alef-arab.fina/hah-arab
  * alef-arab.fina/khah-arab

* Tuned the following kerning pairs:
  * reh-arab.fina/jeem-arab.init
  * reh-arab.fina/tche-arab.init
  * reh-arab.fina/hah-arab.init
  * reh-arab.fina/khah-arab.init
  * reh-arab.fina/seen-arab.init
  * reh-arab.fina/sheen-arab.init
  * reh-arab.fina/sad-arab.init
  * reh-arab.fina/dad-arab.init
  * zain-arab.fina/tcheh-arab.init
  * zain-arab.fina/jeem-arab.init
  * zain-arab.fina/hah-arab.init
  * zain-arab.fina/khah-arab.init
  * zain-arab.fina/seen-arab.init
  * zain-arab.fina/sheen-arab.init
  * zain-arab.fina/sad-arab.init
  * zain-arab.fina/dad-arab.init
  * waw-arab/alef-arab
  * waw-arab/kaf-arab
  * waw-arab/gaf-arab
  * waw-arab/farsiyeh-arab.init
  * waw-arab/beh-arab.init
  * waw-arab/feh-arab.init
  * waw-arab/lam-arab.init
  * waw-arab/alef-arab.isol
  * reh-arab.fina/meem-arab.init

## v1.0.0 - Initial release

* The whole font was rebuilt using a known standardized font with all ligatures, kerning, and positions already implemented
* All characters and glyphs that are not used in Persian texts were removed
* The remaining characters were all harmonized
* Left and right bearings for almost all characters were readjusted and unified to avoid unexpected kerning behaviours
* Thousands of unused kerning/positioning items in various tables were removed
* Hundreds of new kerning pairs and positioning instructions were added to account for all the missing cases
* New classes were defined to be used in kerning situations that can benefit from a uniform kerning parameter for a class of characters instead of creating individual pairs for each one
* Unsupported tables were removed from the font properties
* Unused Unicode character-set ranges were removed from the font and only the ranges that are actually used were kept in the font
* The shapes of a few characters, such as feh-arab.init, qaf-arab.init, feh-arab.medi, qaf-arab.medi, etc. were tweaked to improve their connections with the next character in a word. This makes a lot more sense when the font is used in small sizes where those initial letters can appear as if they were colliding with the next letter in a word. Now, the few pixels that are added to the length of their connectors will allow for a clean and clear distinction of those letters in smaller sizes
* All available glyphs have advanced hints, whereas in the original design, no hint was available for any
* The positions for the vowels were explicitly defined and adjusted for all available glyphs. The original font did not have explicit instructions for the placement of the vowels. As a result, the vowels used to be placed as far up in a block or as far down in a block as possible (that was the defaults)
* Several new kerning classes were defined to account for final characters followed by a [zwnj](https://en.wikipedia.org/wiki/Zero-width_non-joiner) character (none existed in the original design); e.g. `خواهم&zwnj;می`
* Several classes were introduced in kerning pairs where a zwnj character is followed by an initial letter (none existed in the original design); e.g. again `خواهم&zwnj;می`
* The left bearings of many characters were readjusted again to account for the kerning of specific classes, so unexpected behaviours would be eliminated from all possible pairs when kerning is applied
* The right bearings of several characters that had very tall glyphs with wide tops, such as alef with a madda-above, kaf, gaf, and others, were adjusted so when they are paired with short or low characters on their right side, the kerning will not behave unexpectedly with a large, excess white space
* Although the top diacritics were lowered to sit well on top of each glyph, they were placed on three overall grid lines, one for the letters that are very low in height, another for the letters that are above the base but not way up there, and the last grid line for the tallest glyphs. Therefore, the appearance of the diacritics, if used extensively, will not create a messy look, and still follow a clean and defined rule
* The descender part of the character ARABIC DAMMA, i.e. $064F, has been shortened by a few pixels to avoid collision with following letters when the second letter has one or more dots on top
* The small yeh on top of heh, also known as yeh-cheh, was corrected and does no longer look like hamzeh any more
* Superscript glyphs for one, two, and three were made using the existing glyphs
* The following fractions were made out of the available glyphs: 1/2, 1/4, and 3/4
* The Unicode characters to signal right-to-left, left-to-right, and several other control characters were added (they were mostly missing in the original design)
* Added the most basic Latin alphabets and the most commonly-used symbols and special characters from various Unicode blocks
* A clear license notice was added to signal the legal status of EB-Ketab in contrast to N-Ketab that was missing any license notice. The chosen license was SIL OFL that is suitable for this project and its future developments, if there would be any
* A new unique, reserved font name was introduced, i.e. EB-Ketab, to distinguish this project from the original font
* All font validation checks were carried out and problems were resolved. The font checks out the validation process with no error message now
* The PANOSE code was changed from 0-0-4-0-0-0-0-0-0-0 to 2-11-5-0-0-0-0-0-0-0
* A sample text was added to the properties of the font (did not exist in the original)
