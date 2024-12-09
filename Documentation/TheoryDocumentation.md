# Theory Documentation
Reference documentation for पत्थर सिद्धांत (stone theory), a hindi/devanagari machine steno theory.

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

Most English theories tend to default to a "greedy" approach to what to include in a syllable stroke; meaning, try to include as many sounds in the stroke as possible using the RHS to capture more of the word (ex. "falter" might be stroked as TPAUL/T-R (non-greedy) or TPAULT/-R (greedy)).  For Hindi, I have so far found it bemore natural to use a non-greedy approach.  I have found that a more greedy approach did not seem to work as well as it does in English Steno.  It is possible that this will make the theory more stroke intensive.  We will be looking for opportunities to incorporate short cuts and possible some greedy rules to reduce the number of strokes needed.

### Consonant Sounds and Spelling

### Left Hand Side

Left hand side means here the consonant sound when beginning a word or syllable and therefore stroked using the left hand steno keys.

#### Left Hand Side Base Consonants

Left Hand Side for the base consonant sounds (i.e. the consonants in the alphabet only).  Listed in dictionary order.

|Sound-Devanagari|Sound-Roman|STENO|Note|
|:---:|:---:|:---:|---|
|क,क़|k-,q-|K|Use for both in words.|
|ख,ख़|kh-|KWH|Use for both in words.|
|ग,ग़|g|KP|Use for both in words.|
|घ|gh|KPH||
|च|ch|KH||
|छ|chh|KHR||
|ज|j|SKWR||
|ज्ञ|gy-|KPW|Included in the alphabet in many textbooks, but technically a conjuct of ज and ञ.  Sound is irregular in Hindi (like Gaya).|
|ज़|z|SWR||
|झ|jh|SKWHR||
|ट|t|TR||
|ठ|th|THR||
|ड|d|TKR||
|ड़|r|WR|Not typically found in word initial position.|
|ढ|dh|TKHR||
|ढ़|rdh|WHR|Not typically found in word initial position.|
|ण|n-|TPH|Not typically found in word initial position. On the rare occassion when this starts a syllable, it will be stroked same as न.|
|त|t|T||
|थ|th|TH||
|द|d|TK||
|ध|dh|ध||
|न|n|TPH||
|प|p|P||
|फ|ph|PHR||
|फ़|f|फ़||
|ब|b|PW||
|भ|bh|PWH||
|म|m|PH||
|य|y|KWR||
|र|r|R||
|ल|l|HR||
|व|v|W||
|श,ष|sh-|SH|Use for both in words.|
|स|s|S||
|ह|h|H||

#### Conjunct Consonant Rule

Split a word intro strokes on a conjunct character.  This means that when there is a mid-word conjunct, the first member of conjunct ends a syllable stroke and the second member conjunct starts the next syllable stroke.  The primary exception to this rule will be 

Note: This is the current rule, but is under consideration.  It is possible that strokes will be created where the entire conjunct is used to start the second syllable either as an alternative stroke or when there is a clear LHS stroke option for the conjunct (ex. स्क = SK, see [Additional Left Hand Side Consonant Sounds/Spellings](#additional-left-hand-side-consonant-soundsspellings))

#### Additional Left Hand Side Consonant Sounds/Spellings

Left Hand Side for additionaly consonant sounds (i.e. consonant sounds beyond the alphabet only such as combined sounds)

Unless noted, the below strokes will respect the [Conjunct Consonant Rule](#conjunct-consonant-rule).  Therefore, the below will always be used for start of word, but may not always be used when splitting syllables.  When a conjunct stroke does not follow the conjunct consonant rule, that means when found mid-word the stroke will start the next syllable rather than being split.

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
|दृ|dr-|TKR||
|वृ|vr-|WR|**Decide if this is beginning of word only.  When in the middle of a word, it could also be split.** This will conflict directly with ड़ so we'll see if this works out.|
|कृ|kr-|KR||
|स्कृ|skr-|SKR||
|गृ, ग़ृ|gri|KPREU||
|घृ|ghr-|KPHR||
|नृ|nr-|TPHR||
|पृ|pr-|PR||
|तृ|tr-|TR||
|बृ|br-|PWR||
|मृ|mr-|PHR||
|हृ|hr-|R|The ह is ignored.  Potential for conflict with र in otherwise identical words.  However, not very common in words.|
|ऋ|r-|R|Vowel ऋ when it starts a syllable by itself rather than as a maatra attached to another consonant (ex. ऋतु).|

### Vowel Sounds and Spelling

#### Vowel Omission

A quick note on the default _a_ sound in Hindi.  We will follow the convention of ommiting the vowel in these strokes.  So, for example a syllable that consists of consonant-defaul_a_sound-consonant or consonant-default_a_sound will be stroked using just the left hand side, ommiting the vowel stroke, and the right hand side consonant if required.  However, when the default _a_ vowel sound begins a syllable/word or ends a word, it will be included in the stroke.

#### Vowel Sounds and Spelling - Concepts

When stroking a word, you will typically be stroking full syllables (beginning consonant sound + vowel sound + ending consonant sound [if any]).  The output will be an appropriate Devanagari _maatra_ attached to the beginning consonant for that vowel sound.  Reminder: The default _a_ (schwa) sound is automatically assumed and therefore no maatra would appear.  This would apply to most syllables you stroke.  

However, we also have to consider the following cases:
1. How is a vowel sound strokes when the syllable starts with a vowel sound.
2. Is a vowel sound stroked any differently when there is no ending consonant to the syllable?
3. Is a vowel sound stroked any differently when the final syllable in the word ends in an audible vowel sound?

Having different stroke patterns for the same vowel sound in cases like these is used by some English theories to help avoid [word-boundary errors](https://www.artofchording.com/multistroke/prefixes-and-suffixes.html#word-boundary-errors).  Therefore, we will do the same in this theory when needed to avoid word-boundary errors.

We also have to consider nasalization.  Both vowel and consonant sounds can have nasalisation indicated in Devanagari by Bindu/Chandrabindu for vowel nasalisation and Anusvar (looks the same as a Bindu) for consonant nasalization.  Nasalization will typically be treated as the same as adding an "n" sound, with the exception that for some words consonant nasalisation will be treated as adding an "m" sound.

Keeping this in mind, our documentation for vowel sounds will include:
- Base: This will document the standard way of stroking a vowel sound in a syllable
- Nasalization: How to add nasalisation to a vowel sound or consonant sound
- Vowel sound rules when vowel sound is at the beginning of a syllable
- Vowel sound rules when vowel sound is at the beginning of a word
- Vowel sound rules when a vowel sound is at the ending of a syllable
- Vowel sound rules when a vowel sound is at the ending of a word

#### Base

Standard Vowel Sounds (Added to left hand consonant).  The Devanagari character is shown for clarity, but remember that in a syllable the sound is commonly represented as a maatra.

|Sound-Devanagari|Sound-Roman|STENO|Note|
|:---:|:---:|:---:|---|
|अ|a|*NONE*|This is typically omitted.|
|आ|aa|AU||
|इ|i|EU||
|ई|ee|AOE||
|उ|u|AO||
|ऊ|oo|KHR|Long "u" sound|
|ऋ|r|R|We use "R" to represent this sound in words, including in the rare case where the ऋ sound starts a syllable by itself (ex. ऋजुता). When written as a maatra attached to a consonant (तृ, कृ, etc.) it tends to behave like a conjunct (see [Additional Left Hand Side Consonant Sounds/Spellings](#additional-left-hand-side-consonant-soundsspellings)).  When fingerspelling ONLY, this maatra is added to the stroke using "E" - see [finger spelling](#finger-spelling) for details.|
|ए|e|AEU|Long "a" sound.|
|ऐ|ai|AOEU||
|ओ|o|O||
|औ|au|AOU||

#### Nasalisation

Nasalisation is treated as an "n" sound for most nasalisation.  For a small number of words, consonant nasalisation would be represented as an "m" sound (ex. लम्बा which can also be written in Devanagari as लंबा).

Note: In general, this theory will output a conjunct in preference to anusvar for words like लम्बा (also written as लंबा) and हिन्दी (also written as हिंदी), where both versions are commonly recognized.  For words where anusvar is now more commonly seen and the conjunct might be confusing an anusvar will be output.

#### Vowel Sound - Beginning of Word

No special rules yet.

#### Vowel Sound - Beginning of Syllable

No special rules yet.

#### Vowel Sound - End of Word

TODO: Add these.

#### Vowel Sound - End of Syllable

TODO: Add these. (Not sure if there are any just for syllable.  I think so.)

#### Additional

Additional here means vowel sounds (such as diphthongs) beyond the base vowel sounds when then appear in a word/syllable.

#### Special

Special here refers to rules for vowel sounds when they appear in specific places in a word.  This is typically done to avoid conflicts or issues with word boundaries.

### Right Hand Side

Right hand side means here the consonant sound when ending a word or syllable and therefore stroked using the right hand steno keys.

#### Right Hand Side Base Consonants

Right Hand Side for the base consonant sounds (i.e. the consonants in the alphabet only)

Notes: 
- Remember that this theory is typically [non-greedy](#greedy-or-non-greedy).  Therefore, when the base consonants appear mid-word, they will typically start the next syllable stroke and therefore will use the [Left Hand Side rules](#left-hand-side-base-consonants).  Another way to think about this is that these will typically be end of word strokes.
- Aspirated characters _may_ be split mid word.  See notes.
- Not all consonants have a right hand side stroke.  As words with required right hand side consonant strokes are added, these rules will be updated to include them.

|Sound-Devanagari|Sound-Roman|STENO|Note|
|:---:|:---:|:---:|---|
|ब|-b|-B||
|च|-ch|-FP||
|छ|-ch|-FP||
|द|-d|-D||
|ग|-g|-G||
|ज|-j|-PBLG||
|झ|-j|-PBLG||
|क, क़|-k|-BG||
|ख, ख़|-k|-BG||
|ल|-l|-L||
|म|-m|-PL||
|न|-n|-PB||
|प|-p|-P||
|ढ़|-rd|-RD||
|ड़|-r|-R||
|ड़|-r|-R/-R|When full word conflicts|
|र|-r|-R||
|श|-sh|-GS||
|ष|-sh|-GS||
|थ|-th|-GT||
|ट|-t|-T||
|ठ|-t|-T|tentative, consider if a syllable split rule is needed|
|त|-t|-T||
|ज़|-z|-Z||

#### Additional Right Hand Side Consonant Sounds/Spellings

Right Hand Side for additional consonant sounds (i.e. consonant sounds beyond the alphabet only such as combined sounds).

Unless noted, the below strokes will respect the [Conjunct Consonant Rule](#conjunct-consonant-rule).  Therefore, the below will always be used for start of word, but may not always be used when splitting syllables.  When a conjunct stroke does not follow the conjunct consonant rule, that means when found mid-word the stroke will start the next syllable rather than being split.

TODO: Review each of the below to determine which follow the Conjunct Consonant Rule.

|Sound-Devanagari|Sound-Roman|STENO|Note|
|:---:|:---:|:---:|---|
|आय|-aay|AU/AO\*E|Specifically solving for अध्याय|
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

### Consonant-Vowel Word Parts and Blends

These rules cover special cases where a specific stroke is used on the left or right hand side with a specific combination consonants and vowels.  These rules may exist to avoid conflicts and word boundary issues, or to shorten the number of strokes needed to produce words with these combinations.

### Prefixes and Suffixes

Specific and common prefix and suffix strokes for highly used prefixes and suffixes in the Hindi language.

#### Prefixes

Prefixes

#### Suffixes

Suffixes

### Mandatories and Briefs

A brief is using a single stroke to write either an entire multi-syllable word or multiple syllables of a larger word.  These will be used for high volume words to reduce the number of strokes.  Where possible, this will follow patterns to make these briefs easier to remember.

A mandatory is simply a brief to write a word where that brief is the *only* way to write the word.  This is typically done to avoid conflicts where that sound is used in other words.

Note: A brief can also be created for a whole phrase (multiple words).  This is less common, but can be very helpful for high volume phrases.

#### Mandatories

Mandatory list

#### Briefs

Briefs list

#### Phrase Briefs

Phrase briefs

### Finger-spelling

When spelling out a proper name, or to write a word that isn't in the dictionay yet, fingerspelling may be used.  Rather than repeat the base consonant and vowel tables above, we will simply document the finger-spelling rules and note consonants or vowels that require a different stroke for fingerspelling.  Note that fingerspelling strokes can also be used to add maatras, virama, etc.  So, "finger-spelling" is quite a bit more inclusive than it is in English steno.  This reflects that the Devanagari script is more "syllable" in nature by default.  In other words, finger-spelling should be quite a bit more efficient in Hindi steno than it is in English steno.

1. \*R is added to each base consonant or vowel to fingerspell it.  This will append the character to whatever word you are writting.
2. To end a word you will need to manually stroke a space character (SP-Z).
3. You may have noticed in [Left Hand Side Base Consonants](#left-hand-side-base-consonants) that some strokes cover more than one character (ex. क and क़ both use "K").  This won't work for fingerspelling so the following consonants require a special stroke.  The following table documents base consonants that require a separate left hand side stroke for fingerspelling only.

|Sound-Devanagari|Sound-Roman|STENO
|:---:|:---:|:---:|
|क़|q-|KW*R|
|ख़|kh-|WH*R|
|ग़|g|KPHR*R|
|ष|sh-|SKHR*R|

4. Maatras, nasalisation, visarg, halant, anusvaar can be added to your finger-spelling stroke as follows: TODO: Document.

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




