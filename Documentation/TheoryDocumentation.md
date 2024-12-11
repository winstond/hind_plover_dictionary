# Theory Documentation
Reference documentation for पत्थर सिद्धांत (stone theory), a hindi/devanagari machine steno theory.

## Development Status of This Theory

This theory and this documentation should very much be considered "in development".  Although many of the below rules are mature enough that I don't expect them to change, there are many that I would consider tentative so please do expect potentially significant change to the rules/documentation of this theory.

## About Hindi

Hindi is written in a script called [Devanagari](https://hindilanguage.info/devanagari/).  Devanagari consists of consonants and stand-alone vowels.  However, when written vowels most commonly appear in words as a maatra sign.  Therefore, when writing hindi each consonant has a form of the consonant+matra representing the consonant with the vowel sound.

Hindi Devanagari is considered a mostly phonetic script, meaning the written word accurately reflects the pronunciation.  Therefore, if you learn the Devanagari script then sounding out words in Hindi is much easier than for example English where the same grouping of letters may have different sounds when spoken (ex. pour, hour).

For the remainder of this document, it is assumed that the reader knows Hindi and can read Devanagari.

## Theory Reference

### Introduction

Writing Hindi Devanagari is possible, but quite painful using a keyboard.  Many Hindi speakers when typing don't even bother with Devanagari and symply type the roman letter equivalents (usually refered to as "romanagari").  Some phone keyboards will offer to replace romanagari with devanagari so that can be a workaround.  Then again, romanagari doesn't always work to uniquely identify devanagari words as Hindi has sounds that don't exist in English so romanagari is at best an approximate.

I was looking for a way to write Devanagari with at least some reasonable speed on the computer.  Fortunately, the Plover CAT software (see below description) supports outputing any unicode character.

Although Hindi is quite different from English in many ways, fortunately there is a large overlap in sounds (there are only a handful of sounds in Hindi that don't exist in English), and Hindi, like English, does not have the kind of "tone rules" that you might find in languages like Mandarin.  Therefore, it turns out that the same Steno layout used for English can be adapted to use for Hindi!

This is a brand new theory.  I have no idea what the speed capability might be.  If this theory can make writing Devanagari faster and easier, then I will consider it a success and use it regularly.

If you are here and plan to use this theory, I'd love to hear from you.  If you manage to achieve any speed greater than 60wpm, I definitely want to hear from you! You can find me on the Plover Discord Server, with all conversations about this Steno Theory happening in the \#hindi-हिन्दी channel.  See you there!

### Keyboard Layout

There are many types of machine shorthand in the world.  This theory leverages the English machine shorthand system known as [Stenotype](https://en.wikipedia.org/wiki/Stenotype), and also known as the [Ward Stone Ireland layout](https://plover.wiki/index.php/Ward_Stone_Ireland_layout).

For the balance of this documentation, it is assumed that you are familiar with Stenotype and the standard Ireland layout.

### Machine Stenography and CAT software

To use this or any machine steno theory to write on your computer you require a steno machine with the Ireland layout (there are many including enthusiast machines designed as keyboards), and CAT (Computer Aided Translation) software.  

For the CAT software, there are a number of professional (and very expensive!) options.  However, this author uses [Plover](https://plover.wiki/index.php/Beginner%27s_Guide) which is an open-source CAT created by the [Open Steno Project](https://www.openstenoproject.org/) which is completely free to use and works on Windows/MAC/Linux.

For the steno machine, there are professional machines used by court reporters (which tend to be quite expensive).  However, there are also hobbyist keyboards designed with the Ireland layout that are inexpensive and easy to use.  You can see some listed on the [Commercially available hobbyist writers](https://plover.wiki/index.php/Supported_hardware#Commercially_available_hobbyist_writers) on the Plover website.

Please note: This author uses only Plover CAT software.  Plover uses JSON format to define the dictionary.  Most professional CAT software uses a different text file format for their dictionaries.  It should not be terribly difficult to convert the dictionaries found here to another format.  However, that is outside the scope of this documentation and this project.

For the balance of this document, it will be assumed that you have a steno machine with the Ireland layout, have a CAT installed, and know how load a steno dictionary.

### Greedy or Non-Greedy

Most English theories tend to default to a "greedy" approach to what to include in a syllable stroke; meaning, try to include as many sounds in the stroke as possible using the RHS to capture more of the word (ex. "falter" might be stroked as TPAUL/T-R (non-greedy) or TPAULT/-R (greedy)).  For Hindi, I have so far found it to be more natural to use a non-greedy approach.  I have found that a more greedy approach did not seem to work as well as it does in English Steno.  It is possible that this will make the theory more stroke intensive.  I will be looking for opportunities to incorporate shortcuts and possibly add greedy rules to reduce the number of strokes needed.

### Consonant Sounds and Spelling

### Left Hand Side

Left hand side means here the consonant sound when beginning a word or syllable and therefore stroked using the left hand steno keys.

#### Left Hand Side Base Consonants

Left Hand Side for the base consonant sounds (i.e. the consonants in the alphabet only).  Listed in dictionary order.

|Sound-Devanagari|Sound-Roman|STENO|Note|
|:---:|:---:|:---:|---|
|क,क़|k-,q-|K|Use for both in words.|
|ख,ख़|kh-|KWH|Use for both in words.|
|ग,ग़|g-|KP|Use for both in words.|
|घ|gh-|KPH||
|च|ch-|KH||
|छ|chh-|KHR||
|ज|j-|SKWR||
|ज्ञ|gy-|KPW|Included in the alphabet in many textbooks, but technically a conjuct of ज and ञ.  Sound is irregular in Hindi (like Gaya).|
|ज़|z-|SWR||
|झ|jh-|SKWHR||
|ट|t-|TR||
|ठ|th-|THR||
|ड|d-|TKR||
|ड़|r-|WR|Not typically found in word initial position.|
|ढ|dh-|TKHR||
|ढ़|rdh-|WHR|Not typically found in word initial position.|
|ण|n-|TPH|Not typically found in word initial position. On the rare occassion when this starts a syllable, it will be stroked same as न.|
|त|t-|T||
|थ|th-|TH||
|द|d-|TK||
|ध|dh-|TKH||
|न|n-|TPH||
|प|p-|P||
|फ|ph-|PHR||
|फ़|f-|TP||
|ब|b-|PW||
|भ|bh-|PWH||
|म|m-|PH||
|य|y-|KWR||
|र|r-|R||
|ल|l-|HR||
|व|v-|W||
|श,ष|sh-|SH|Use for both in words.|
|स|s-|S||
|ह|h-|H||
|ऋ|ri-|REU|NOTE: ऋ is not a consonant, but for purposes of Steno behaves as one when used as a standalone character in a word.  See [Vowel Sound - Base](#vowel-sound---base) for more information about ऋ.|

#### Conjunct Consonant Rule

The conjunct consonant rule is that you split a word into syllable strokes on a conjunct character.  This means that when there is a mid-word conjunct, the first member of conjunct ends the first syllable stroke and the second member of the conjunct starts the next syllable stroke.  There will be exceptions to this rule.

Here is a nonexhaustive list of conjuncts that will split mid word:

TODO: Increase the number of examples, provide sample words for each.

|Sound-Devanagari|Sound-Roman|STENO|Note|
|:---:|:---:|:---:|---|
|ब्द|-bd|-B/TK||
|ब्ध|-bdh|-B/TKH||
|ष्ट|-sht|SH/TR|Sample words/strokes; अष्टक: AGS/TR-BG, कुदृष्टि: KAO/TKREUGS/TEU|

Some non-conjunct consonants (particularly aspirated consonants) may also follow the conjunct consonant rule.  For example, ढ़ when found mid word will be stroked as -RD/H.  Here is a list of non-conjunct consonants that will follow the conjunct consonant rule.

TODO: Increase the number of examples, provide sample words for each.

|Sound-Devanagari|Sound-Roman|STENO|Note|
|:---:|:---:|:---:|---|
|ढ़|rdh|-RD/H|When splitting syllables, end last syllable -RD and begin next syllable on H|

Here is a list of a additional situations where we will split a complex sound between syllables and can be considered to follow the conjunct consonant rule:

TODO: Increase the number of examples, provide sample words for each.

|Sound-Devanagari|Sound-Roman|STENO|Note|
|:---:|:---:|:---:|---|
|अंग|-ng|-\*PBG/KP|When splitting syllables, this usually sounds like ng on the end of the first syllable and g on the beginning of the next|
|अंघ|-ngh|-\*PBG/KPH|When splitting syllables, this usually sounds like ng on the end of the first syllable and gh on the beginning of the next|

Exceptions: Some conjuncts do NOT follow the conjunct consonant rule.  When they appear mid word, they will start the second syllable rather than being split.  The following conjuncts do not follow the conjunct consonant rule:

TODO: Increase the number of examples, provide sample words for each.

|Sound-Devanagari|Sound-Roman|STENO|Note|
|:---:|:---:|:---:|---|
|त्र and ट्र|tr-||When splitting syllables, use त्र for the following syllable (so TR) rather than splitting between (-T/R)|

TODO: Review these.  Confirm if they follow the rule or not:
|झ|jh|-PBLG or -PBLG/H|When splitting syllables and no matra, allow for both SKWHR and SKWHR/H|
|द्ध|ddh|-D/TKH or -D/H + matra if necessary|Works middle or end of word.  Suggest making strokes for both.|

TODO: Consider to what extent the theory should support multiple options (i.e. allow word with conjuncts or conjunct-like sounds to have multiple theory strokes, one with the split, another without).

#### Additional Left Hand Side Consonant Sounds/Spellings

Left Hand Side for additionaly consonant sounds (i.e. consonant sounds beyond the alphabet only such as combined sounds)

Unless noted, the below strokes will respect the [Conjunct Consonant Rule](#conjunct-consonant-rule).  Therefore, the below will always be used for start of word, but may not always be used when splitting syllables.

TODO: Review each of the below to determine which follow the Conjunct Consonant Rule.

|Sound-Devanagari|Sound-Roman|STENO|Note|
|:---:|:---:|:---:|---|
|भ्र|bhr-|PWHR|Does not follow conjunct consonant rule.|
|ब्ल|bl-|PWHR|Rare.  Only used beginning of word.|
|द्व|dv-TKW||
|ग्र|gr-|KPR||
|क्र|kr-|KR||
|क्ष|ksh-|SKH||
|प्र|pr-|PR||
|श्र|shr-|SHR||
|स्क|sk-|SK||
|स्न|sn-|STPH||
|स्प|sp-|SP||
|स्त or स्ट|st-|ST||
|स्थ|sth-|ST||
|स्व|sv-|SW||
|स्य|sy-|SAOE/KWR|Sounds like see/ya|
|त्र and ट्र|tr-|TR|Using TR for now, which risks conflict with ट.  Monitor for conflicts.|
|व्य|vy-|KPWR|Beginning of word only (see [Conjunct Consonant Rules](#conjunct-consonant-rules).).  This typically sounds like "ve/ya" (except when followed by ng (nasalisation+ग) where it just sounds like veng)|
|दृ, वृ, कृ, स्कृ, गृ/ग़ृ, घृ, नृ, पृ, तृ, बृ, मृ, हृ/ऋ|dri-, vri-, kri-, skri-, gri-, ghri, nri, pri, tri, bri, mri, ri|\*ri|Note: Essentially this will be consonant+"ri".  See [Vowel Sound - Base](#vowel-sound---base) for explanation of how ऋ behaves both as a maatra and a standalone letter.|

### Vowel Sounds and Spelling

#### Vowel Omission

A quick note on the default _a_ sound in Hindi.  We will follow the convention of ommiting the vowel in these strokes.  So, for example a syllable that consists of consonant-defaul_a_sound-consonant or consonant-default_a_sound will be stroked using just the left hand side, ommiting the vowel stroke, and the right hand side consonant if required.  However, when the default _a_ vowel sound begins a syllable/word or ends a word, it will be included in the stroke.

#### Vowel Sounds and Spelling - Concepts

Vowel sounds will typically be stroked using the thumbs of each hand on the vowel keys on the steno machine (the bottom row).

When stroking a word, you will typically be stroking full syllables (beginning consonant sound + vowel sound + ending consonant sound [if any]).  The output will be an appropriate Devanagari _maatra_ attached to the beginning consonant for that vowel sound.  Reminder: The default _a_ (schwa) sound is automatically assumed and therefore no maatra would appear.  This would apply to most syllables you stroke.  

However, we also have to consider the following cases:
1. How is a vowel sound stroked when the syllable starts with a vowel sound.
2. Is a vowel sound stroked any differently when there is no ending consonant at the end of the syllable (i.e. the syllable ends with a vowel sound)?
3. Is a vowel sound stroked any differently when the final syllable in the word ends in a vowel sound?

Having different stroke patterns for the same vowel sound in cases like these is used by some English theories to help avoid [word-boundary errors](https://www.artofchording.com/multistroke/prefixes-and-suffixes.html#word-boundary-errors).  Therefore, we will do the same in this theory when needed to avoid word-boundary errors.

We also have to consider nasalization.  Both vowel and consonant sounds can have nasalization indicated in Devanagari by Bindu/Chandrabindu for vowel nasalization and Anusvar (looks the same as a Bindu) for consonant nasalization.  Nasalization will typically be treated as the same as adding an "n" sound, with the exception that for some words consonant nasalisation will be treated as adding an "m" sound.

Keeping this in mind, our documentation for vowel sounds will include:
- Base: This will document the standard way of stroking a vowel sound in a syllable
- Nasalization: How to add nasalisation to a vowel sound or consonant sound
- Semi-Vowels: Rules for how य and ह affect vowel sounds
- Vowel sound rules when vowel sound is at the beginning of a syllable
- Vowel sound rules when vowel sound is at the beginning of a word
- Vowel sound rules when a vowel sound is at the ending of a syllable
- Vowel sound rules when a vowel sound is at the ending of a word
- Special cases, such as vowel+consonant end of word rules and consonant+vowel blend rules

#### Vowel Sound - Base

Standard Vowel Sounds (Added to left hand consonant).  The Devanagari character is shown for clarity, but remember that in a syllable the sound is commonly represented as a maatra.

|Sound-Devanagari|Sound-Roman|STENO|Note|
|:---:|:---:|:---:|---|
|अ|a|*NONE*|This is typically omitted.|
|आ|aa|AU||
|इ|i|EU||
|ई|ee|AOE||
|उ|u|AO||
|ऊ|oo|U|Long "u" sound|
|ऋ|r|REU|Vocalized using a short "i" sound in addition to the "r" so "ri".  In Steno, this is treated more as a consonant+vowel matra pair (specifically रि) due to its pronunciation.  When written as a maatra attached to a consonant (तृ, कृ, etc.) therefore, it tends to behave like a conjunct (see [Additional Left Hand Side Consonant Sounds/Spellings](#additional-left-hand-side-consonant-soundsspellings)).  When fingerspelling ONLY, this maatra is added to the stroke using "E" - see [finger spelling](#finger-spelling) for details.|
|ए|e|AEU|Long "a" sound.|
|ऐ|ai|AOEU||
|ओ|o|O||
|औ|au|AOU||

#### Vowels Sound - Nasalisation

Nasalisation is treated as an "n" sound for most nasalisation.  For a small number of words, consonant nasalisation would be represented as an "m" sound (ex. लम्बा which can also be written in Devanagari as लंबा).

Note: In general, this theory will output a conjunct in preference to anusvar for words like लम्बा (also written as लंबा) and हिन्दी (also written as हिंदी), where both versions are commonly recognized.  For words where anusvar is now more commonly seen in print and therefore the conjunct might be confusing an anusvar will be output.

#### Vowel Sound - Semivowels

The semivowels ह and य can have some effect on the pronunciation of vowel sounds.  The following rules cover these cases:

|Sound-Devanagari|Sound-Roman|STENO|Note|Reviewed|
|:---:|:---:|:---:|---|---|
|बह, रह, लह, मह, दह, जह, शह, षह, चह|be, re, le, me, de, je, she, she, che|AEU|When ह combines with certain consonants the resulting sound is an ए.  The general rule is: "When ह is not followed by a full vocalic sound (i.e. it only has the default अ after it), the अ pronunciation changes to ए insteadl.  See also: [Vowel Sound - End of Word](#vowel-sound---end-of-word) for end of word behavior.|Yes|
|आय|-aiya|AOEU|Rule: य semivowel after आ changes the sound to ऐ.  Examples: 1. शायद - the आय sounds like one type of pronunciation of ऐ so stroke is SHAOEU/KWR-D. 2. बनाया would be PW/TPHAOEU/KWRAU.  Follow this rule by pronunciation.  Example Words: किफ़ायत, उपाय, इलायची|YES|

#### Vowel Sound - Beginning of Word

No special rules yet.

#### Vowel Sound - Beginning of Syllable

No special rules yet.

#### Vowel Sound - End of Word

Rules for vowel/semivowel sounds and the end of a word.  When necessary, these may use different strokes than the vowel in the beginning or middle of a word to avoid word-boundary issues.

TODO: All of these need to be reviewed and tested to confirm when a separate end of word stroke is needed to avoid word boundary errors.

|Sound-Devanagari|Sound-Roman|STENO|Note|Reviewed|
|:---:|:---:|:---:|---|---|
|अ|-a|A|When the default अ sound is pronounced at the end of a word, add A to the consonant stroke.||
|आह|-aa|AU|End of Word Rule: The sounds enough like आ, that we simply use the normal आ stroke patter. TODO: Review this.  Should all words ending in the आ sound have a unique stroke to avoid word boundary errors with words beginning with आ?||
|ए|-e|A\*EU|||
|ई|-ee|AO\*E|Note: End of sentence or end of syllable only.  Example:डाई - sounds like ah-ee||
|आइ|-aai|AU/EU|diphthong rule||
|आई|-aaee|AU/AOE|diphthong rule||
|ओह|-oh|O|Seems to be pronounced like a slightly long "o".  We'll simply use the normal stroke for ओ, and keep this as an orthography rule if necessary.||
|बह, रह, लह, मह, दह, जह, शह, षह, चह|be, re, le, me, de, je, she, she, che|A\*EU|See [Vowel Sound - Semivowels](#vowel-sound---semivowels) for details on this behavior.  This is treated as another application of ए sound end of word.|YES|

#### Vowel Sound - End of Syllable

|Sound-Devanagari|Sound-Roman|STENO|Note|
|:---:|:---:|:---:|---|

#### Additional

Additional here means vowel sounds (such as diphthongs) beyond the base vowel sounds when then appear in a word/syllable.

#### Special

Special here refers to rules for vowel sounds when they appear in specific places in a word.  This is typically done to avoid conflicts or issues with word boundaries.

|Sound-Devanagari|Sound-Roman|STENO|Note|
|:---:|:---:|:---:|---|
|आंघ and आंग|aang|AUPBG|End of Word Rule: Nasalisation + G or GH. (When found mid word, this pattern will follow the [conjunct consonant rule](#conjunct-consonant-rule) (i.e. the "n" sound will end a syllable and the "g" sound will start the next.|
|आह|aah|AU/HA|End of word rule|

### Right Hand Side

Right hand side means here the consonant sound when ending a word or syllable and therefore stroked using the right hand steno keys.

#### Right Hand Side Base Consonants

Right Hand Side for the base consonant sounds (i.e. the consonants in the alphabet only).  Roughly in dictionary order - some items are combined out of order.

Notes: 
- Aspirated characters _may_ be split mid word.  See [Conjunct Consonant Rule](#conjunct-consonant-rule) which also details which aspirated characters are split mid-word.  In the below tables these will be noted as "End of word only."
- Not all consonants have a right hand side stroke.  As words with required right hand side consonant strokes are added, these rules will be updated to include them.

TODO: Review all RHS aspirated characters.  If they follow conjunct consonant rule, add an "End of word only" note below.
TODO: Review nasalisation before all right hand sounds for impact on stroke.

|Sound-Devanagari|Sound-Roman|STENO|Note|
|:---:|:---:|:---:|---|
|क, क़|-k|-BG||
|ख, ख़|-k|-BG||
|ग, ग़, घ|-g|-G||
|ङ|ng|-PBG|Note: Rare|
|च, छ|-ch, -chh|-FP||
|ज, झ|-j, jh|-PBLG||
|ज़|-z|-Z||
|ट, ठ, त|-t|-T||
|ड़, र|-r|-R||
|ढ़|-rd|-RD|Note: End of word only?|
|न, ञ, ण, vowel nasalization|-n|-PB|Note: vowel nasalisation (अँ, आँ, इँ, ईं, etc.) counts as न for end of syllable|
|थ|-th|-GT||
|द, ध|-d, -dh|-D|Note: End of word only?|
|प|-p|-P||
|फ, फ़|-f|-F|TODO: Consider if there is nasalisation before this.|
|ब, भ|-b, -bh|-B|Note: End of word only?|
|म, vowel nasalisation|-m|-PL|Occassionally this may be represented as vowel nasalisation, for example लंबा (also written as लम्बा).  Note: Theory will typically output the conjunct.|
|ल|-l|-L||
|श, ष|-sh|-GS||
|स|-s|-S||

#### Additional Right Hand Side Consonant Sounds/Spellings

Right Hand Side for additional consonant sounds (i.e. consonant sounds beyond the alphabet only such as combined sounds).

Unless noted, the below strokes will respect the [Conjunct Consonant Rule](#conjunct-consonant-rule).  Therefore, the below will always be used for end of word, but may not always be used when splitting syllables.  When a conjunct stroke does not follow the conjunct consonant rule, that means when found mid-word the stroke will start the next syllable rather than being split.

TODO: Review each of the below to determine which follow the Conjunct Consonant Rule.

|Sound-Devanagari|Sound-Roman|STENO|Note|
|:---:|:---:|:---:|---|
|फ़्त|-ft|-FT||
|ग्ध|-gdh|-GD||
|ख़्स|-ks|-BGS|This will conflict with -ksh.  We'll see if it works out.|
|क्ष|-ksh|-BGS||
|क्त, क़्त|-kt|-BGT||
|ल्द|-ld|-LD||
|ल्क|-lk|-L/-BG|Not common.  Using the Phoenix stroke.|
|ल्प|-lp|-L/-P|Doesn't seem to be common.  Using two-stroke pattern same as in some English theories for words like "gulp"|
|एंच|-nch|-FRPB|nasalisation followed by च or छ|
|आँक|-nck|\*PBG||
|न्ध|-ndh|-PBD||
|न्द|-nd|-PBD||
|नफ़|-nd|-FPB|nasalisation + फ़ (rare so using same stroke as nv)|
|उंग|-ng|-PBG|nasalisation followed by a "g" sound ग or घ|
|उंवज|-ng|-FPG|nasalisation followed by a "j", ज|
|आंख|-nk|\*PBG|nasalisation followed by a "k" sound क or ख|
|अंप or आंप|-np|-PB/-P|nasalisation followed by प.  If this is frequent enough make is a single stroke rule instead.|
|आंस|-ns|-PBS|nasalisation followed by स (when स is ending a syllable/word)|
|न्ठ or ओंठ|-nth|-PBGT|nasalisation followed by थ|
|आंत|-nt|-PBT|nasalisation followed by त|
|आंव|-nv|-FPB|nasalisation followed by व|
|आँ|-n|-PB|Nasalisation|
|प्त|-pt|-PT||
|र्ब|-rb|-RB||
|र्भ|-rbh|-RB||
|र्फ|-rf|-FR||
|र्ग|-rg|-RG||
|र्क|-rk|-RBG||
|र्म|-rm|-RPL||
|र्ण|-rn|-RPB||
|र्न|-rn|-RPB||
|र्श|-rsh|-RGS||
|र्त|-rt|-RT||
|र्व|-rv|-FRB||
|ष्ट|-sht|-GTS||
|स्क|-sk|-FBG||
|स्थ|-sth|-GTS|_tentative_ (alternatives: \*GT, \*S)|
|स्त|-st|\*S||
|-bd|ब्द|-BD||
|-bd|ब्ध|-BD||

### Consonant-Vowel Word Parts and Blends

These rules cover special cases where a specific stroke is used on the left or right hand side with a specific combination consonants and vowels.  These rules may exist to avoid conflicts and word boundary issues, or to shorten the number of strokes needed to produce words with these combinations.

### Prefixes and Suffixes

Specific and common prefix and suffix strokes for highly used prefixes and suffixes in the Hindi language.  

#### Prefixes

None defined yet.

#### Suffixes

None defined yet.

### Mandatories and Briefs

A brief is using a single stroke to write either an entire multi-syllable word or multiple syllables of a larger word.  These will be used for high volume words to reduce the number of strokes.  Where possible, this will follow patterns to make these briefs easier to remember.

A mandatory is simply a brief to write a word where that brief is the *only* way to write the word.  This is typically done to avoid conflicts where that sound is used in other words.

Note: A brief can also be created for a whole phrase (multiple words).  This is less common, but can be very helpful for high volume phrases.

#### Mandatories

None defined yet.

#### Briefs

None defined yet.

#### Phrase Briefs

None defined yet.

### Finger-spelling

When spelling out a proper name, or to write a word that isn't in the dictionay yet, fingerspelling may be used.  Rather than repeat the base consonant and vowel tables above, we will simply document the finger-spelling rules and note consonants or vowels that require a different stroke for fingerspelling.  Note that fingerspelling strokes can also be used to add maatras, virama, etc.  So, "finger-spelling" is quite a bit more inclusive than it is in English steno.  This reflects that the Devanagari script is more "syllable" in nature by default.  In other words, finger-spelling should be quite a bit more efficient in Hindi steno than it is in English steno.

1. \*R is added to each base consonant or vowel to fingerspell it.  This will append the character to whatever word you are writting.
2. To end a word you will need to manually stroke a space character (SP-Z).
3. You may have noticed in [Left Hand Side Base Consonants](#left-hand-side-base-consonants) that some strokes cover more than one character (ex. क and क़ both use "K").  This won't work for fingerspelling so the following consonants require a special stroke.  The following table documents base consonants that require a separate left hand side stroke for fingerspelling only:

|Sound-Devanagari|Sound-Roman|STENO
|:---:|:---:|:---:|
|क़|q-|KW\*R|
|ख़|kh-|WH\*R|
|ग़|g|KPHR\*R|
|ष|sh-|SKHR\*R|

4. Maatras, vowel nasalisation, visarg (consonant nasalisation), halant, anusvaar can be added to your finger-spelling stroke as follows:
For all of the below, you are reminded that all finger-spelling includes \*R, so be sure to include that.

- Matra: Simply add the appropriate base vowel stroke as usual.  Note that for fingerspelling ऋ as a matra will be "E" added to the stroke.
- Vowel nasalisation: Add -B to your stroke (this will put the correct bindu or chandrabindu depending on the vowel matra).
- Anusvar (consonant nasalization): Add -PB to your stroke.
- Halant (used to make conjuncts): Add -S to your stroke
- Visarg (Extra nasalization, looks like a : symbol): Add -G to your stroke.

Examples of various fingerspellings:
त - T\*R (consonant)
ता - TA\*UR (consonant + maatra)
तृ - T\*ER (consonant + ऋ maatra specifically)
ताँ - TA\*URB (consonant + maatra + vowel nasalization)
तं - T\*RPB (consonant + consonant nasalization)
स् - S\*RS (halant for creating a conjunct), स्त: S\*RS/T\*R (showing the production of a conjunct)
तः - T\*RG (consonant + visarg, example word - अतः = A\*R/T\*RG)

Using the above fingerspellings, you should be able to produce almost any hindi word.

NOTE: There is also a "chandra" without the bindu, which is used for transliteration of English words like "coffee" to represent the English "au" sound.  This has not yet been defined for fingerspelling.  Example word: कॉफ़ी (coffee).

### Months, Days, States and Cities

Briefs specifically for months, days, states and well know cities will be here.

### Punctuation

Punctuation is mostly similar to English.  However, Hindi uses the । character for end of sentence.  Also, for greater readability a space is added before punctuation such as ?, !, etc. when used for end of sentence.  I have used strokes common for English Phoenix Theory as that is what I use for English.  Feel free to substitute your own preferences.  Punctuation is kept in a separate dictionary file for convenience.

### Numbers and Ordinals

Number and Ordinal strokes here.  This will include sections with shortcuts for writing lakhs, crore, etc. (commas in the correct places) as well as strokes to add rupee symbol and so forth.  Number strokes will include options to output hindi numerals or arabic numerals.

### Dates and Times

Methods for writing dates and times efficiently.

### Special cases

Can include phone numbers or other alpha-numeric items that are heavily used and follow a specific pattern (Aaadhar number for example).




