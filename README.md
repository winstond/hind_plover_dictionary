# hind_plover_dictionary

## The Latest!
The readme below this section is completely outdated.  It can be disregarded (although it does give a flavor for the strokes that will be used for hindi sounds and characters).

The latest commits include a fingerspelling only dictionary.  Take a look at "hindi_fingerspell.json"  It uses some of the below stroke concepts but everything would need to have \*R added to the stroke or you won't get any output.  If you review it, you'll be able to see how to fingerspell Devanagari characters with mitras, nasalisation, visarg, etc.

We have words!  Take a look at "hindi_words.json" to view our first word dictionary.  It currently has just under 4,000 words.  This is basically UNTESTED.  As in, the strokes will work, but I have no idea if it is full of conflicts or word boundary errors, etc.  Therefore, it could still undergo serious changes if for example I change how I'm stroking a consonant or what have you.

Documentation on the Left Hand Side (beginning consonant sounds), Right Hand Side (ending consonant sounds), Vowels, etc. is a work in progress.  You can view "LHS.md" and "RHS.md" in the repo to see what is documented so far.  It's pretty rough.

## PLEASE NOTE: Undergoing significant updates...
The below documentation refers to release v1.0 which is avaiable for download.  Commits after that will reflect changes that break some of the below documentation.  Please be patient as we create a proper steno dictionary!  Documentation will be updated on next release.

A steno dictionary for writing Hindi in the __Devanagari__ script using Plover Steno.

## Usage

1. Download the hindi.json file (store it wherever you like to keep Plover dictionaries)
2. In Plover, add the dictionary.  It does not require any add-ins.
3. When enabled, you can now output hindi characters using Plover.

Example: To output कीं the stroke would be KAO\*EB.  Breaking this down... K is for the क, AOE adds the की matra (long "e" sound in English), and \*B added to any stroke adds the "bindu" character (or chandrabindu where appropriate).

## Basic operation of this dictionary:

### Words

No "words" are defined.  Therefore you must manually type a space or punctuation to end a word and start a new word or sentence.

### Punctuation

No punctuation is defined here.  Generally, punctuation in Hindi is the same.  I suggest you make a stroke to create a sentence stop.  Hindi uses a vertical bar also know as a pipe character, "|" for end of sentence.  

### Consonants and Vowels:

There is one stroke for each consonant and vowel as follows.  The consonants use the left hand only.  The vowels use vowel keys only.

| Vowel  | Stroke |  | Con Type | Con | Stroke | Con | Stroke | Con | Stroke | Con | Stroke | Con | Stroke |
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
| अ | A |  | Velar: | क/क़ |  K / KW | ख/ख़ | KWH/WH | ग/ग़ | KP/KPHR | घ | KPH | ङ | KPW |
| आ  | AU |  | Palatal: | च | KH | छ | KHR | ज | SKWR | श | SH | ञ | STPH |
| इ | EU |  | Retroflex: | ट | TWR | ठ | TR | ड/ड़ | TKW / WR | ढ/ढ़ | TKPH / TKR | ण | TPHR |
| ई | AOE |  | Dental: | त | T | थ | TH | द | TK | ध | TH | न | TPH |
| उ | AO |  | Labial: | प | P | फ/फ़ | PHR / TP | ब | PW | भ | PWH | म | PH |
| ऊ | U |  | Liquids / Semi-Vowel: | य | KWR | र | R | ल | HR | व | W |  |  |
| ऋ | E |  | Sibilants / Fricative: | श | SH | ष | SKHR | स | S |  |  |  |  |
| ए | AEU |  | Aspirate: | ह | H |  |  |  |  |  |  |
| ऐ | AOEU |  |  |  |  |  |  |  |  |  |  |
| ओ | O |  |  |  |  |  |  |  |  |  |  |
| औ | AOU |  |  |  |  |  |  |  |  |  |  |

### Consonants + Mātrā

Devanagari is syllabic in nature meaning the characters combine consonant + vowel sound.  The vowel sound is indicated by a mātrā form attached to the consonant.

To write consonant + mātrā is simple - just combine the consonant and vowel strokes into one stroke. The only exception is the अ consonant.  In Devanagari that is the default so the consonant with no matra is assumed to have the अ sound after it. Here is an example of all the matra forms for a single consonant, न (similar to "n" sound in English).  The same technique will work with all consonants.

|न|ना|नि|नी|नु|नू|नृ|ने|नै|नो|नौ|
|---|---|---|---|---|---|---|---|---|---|---|
| TPH | TPHAU | TPHEU |TPHAOE |TPHAO |TPHU | TPHE | TPHAEU | TPHAOEU | TPHO | TPHAOU |

### Adding nasalisation with Bindu/Chandrabindu

Nasalisation can be added to the vowel sound by adding special symbols above the character.  This will be either a bindu (looks like a single dot), or a chandrabindu (looks like a half moon with a dot in it).  Whether a vowel nasalisation gets one or the other depends on if the matra form goes "above the line" or not.

To add bindu/chandrabindu nasalisation to your stroke, simply add `*B` to your stroke.  Here is the same table for the letter न, this time adding nasalisation to each with `*B`:

|नँ|नाँ|निं|नीं|नुँ|नूँ|नृँ|नें|नैं|नेौ|नौं|
|---|---|---|---|---|---|---|---|---|---|---|
| TPH\*B | TPHA\*UB | TPH\*EUB | TPHAO\*EB | TPHAO\*B | TPH\*UB | TPH\*EB | TPHA\*EUB | TPHAO\*EUB | TPHO\*B | TPHAO\*UB |

### Adding Visarg

There is a symbol in Devanagari that represents an "echoing" of the vowel sound with an extra puff of breath.  It looks like a colon symbol.  To add that to a stroke, use `*G` added to your stroke.  Here are two examples:

|कः|अः|
|---|---|
| K\*G | A\*G |

### Conjunct Consonants

Finally, Devanagari has a concept of joining consonants together to form a single character  This is typically done to show that the default अ sound should not be used between these two consonants.

To create a conjunct, add `*` to the first consonant stroke - this adds a special character called a _halant_ to the character.  When you stroke the next consonant, the consonants will join.  Here are two common examples:

|स्त|स्क|
|---|---|
| S\*/T | S\*/K |

You might recognize these as they are used in नमस्ते (Namaste, "I bow to you"), and नमस्कार (Namaskār, "I bow to you") - two common greetings.  There are _many_ conjunct consonants used in Hindi words.  This stroke technique will work for most.  However there are some conjuncts that are typically represented by using a dot above the horizontal line instead (see __Other Nasalisation__ below).

### Other nasalisation with anusvaar (consonant, nasal conjuncts, etc.)

An anusvaar (looks like a bindu, single dot above) may be added for other nasalisations as well.  This can be added to a stroke with `*PB`.  Here are two examples:

|कं|खं|
|---|---|
| K\*PB | KWH\*PB |

### Special Characters as second strokes

You may occassionally need to add a special character with a second stroke.  In those cases you can use the following:

|Name|Stoke|Example Stroke|Example Output|
|---|---|---|---|
| Virama | SR\*RBGS | K/SR\*RBGS | क् |
| Bindu | PW\*RBGS | K/PW\*RBGS | कं |
| Chandrabindu | KH\*RBGS | K/KH\*RBGS | कँ |
| Visarg | S\*RBGS | K/S\*RBGS | कः |

And that's it!

## Final thoughts

So, is this a true steno dictionary?  Well, I'll say no since there are no word boundaries and the common "consonant-vowel-consonant" pattern is not used yet.  I think it is certainly possible to create a full Steno theory for Hindi Devanagari, but it will be a lot of work and I'm just learning Hindi.  Once my vocabulary is large enough, I plan to revisit this.  Primarily, what needs to happen is the entire right hand consonants need to be defined so that you may create complete syllables that end in a consonant sound.  Then a much larger dictionary of words will have to be created which will allow for creating the word boundaries.  Topic for another day for me...

Best of luck using this dictionary.  

If you already know English Steno, you may find this dictionary to be a much more efficient way to output Devanagari vs. typing on the keyboard.  Even in my short time developing it, I already find it much more efficient.

I was also gratified that there were enough consonant/vowel sounds that are the same (or close) in English that I was able to use familiar strokes to define them.  If you already know English Steno with a common theory like Plover or Phoenix you will likely notice this and it should make learning these strokes much faster for you.

I did certainly take some liberties!  For example, I eliminated the usual English stroke for hard "g", TKPW.  Never much liked it.  Instead I used KP for the hard "g" sound.  In my English theory KP is used for "ex" prefix so it was available!  Hindi has more consonant sounds than English, and some of them are very similar to each other with one being "aspirated" for example.  I did the best I could to think of logical/intuitive derivative strokes.
