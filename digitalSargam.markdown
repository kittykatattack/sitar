Sitar music notation [learning sitar]
-------------------------------------

### Music notation for the sitar ###

*This article describes how to read and write a modern, open-standard musical notation for the sitar, called [Digital Sargam](https://github.com/sargam/digital). Most of the written notation examples are illustrated by audio MP3 files. They’ve been played on the sitar in the key of D.* To play the audio samples, make sure you are reading this page with a modern web browser, such as [Chrome](https://www.google.com/intl/en/chrome/browser/). To contribute to the Digital Sargam project, [click here](https://github.com/sargam/digital/wiki).

### What is Sargam Notation?

Traditional Indian Classical music notation is called Sargam. The notes used in Sargam notation correspond to the Western Solfa system for describing pitches. In Solfa, the 7 notes of the major scale are Do Re Mi Fa So La Ti. In Sargam notation, these same notes are described as Sa Re Ga ma Pa Dha Ni. The notes of each system correspond to the same pitches; the only difference is the names of the notes.

Here's an example of Sargam notation for the 7 notes of the major scale using the English alphabet:
````
S R G m P D N 
````
<audio controls><source src="audio/1.mp3"></audio>

Assuming that the fist note, Sa, corresponds to middle C, you could write this same scale using staff notation, like this:

![](images/SaReGa.png)

In Sargam notation, upper case letters indicate natural notes, and lowercase letters indicate flat notes. Here's a example of a scale that uses a flat third, flat fourth and flat seventh.
````
S R g m P D n
````
<audio controls><source src="audio/2.mp3"></audio>

Sargam notation is an extremely efficient and easy-to-understand system for describing melodies. Because Indian Classical music is purely melodic and monophonic (there are no chords or harmonies in the strict sense) the Sargam system doesn't need to account for more than one note being voiced at the same time. This means that the system doesn't need a staff; all the notes can remain on a single line. 

To show that notes are in an octave below middle C, Sargam notation adds a dot below the note, like this:

![](images/Sargam1.png)

<audio controls><source src="audio/3.mp3"></audio>

To show that a note is above middle C, a dot is placed above the note, like this:

![](images/Sargam2.png)

<audio controls><source src="audio/4.mp3"></audio>

To demonstrate how this works, here are a series of notes written in Sargam notation that span three octaves:

![](images/SaReGa2.png)

<audio controls><source src="audio/5.mp3"></audio>

Here's how this same phrase would be written using staff notation.

![](images/Sargam3.png)

The notes are the same, but you can clearly see that the Sargam notation is a much clearer and more direct way of describing them. It's easy to read, easy to write, easy to learn, and very focused for the requirements of Classical Indian music. It does become more complex than this when it comes to describing rhythm and structure, but not much more so.

However, as useful as Sargam notation can be, it's never been an essential part of the Indian Classical music tradition. Indian Classical music has always been taught and learnt orally; the use of notation has never been emphasized or required. There are a few very important reasons for this. Many aspects of phrasing and pitch, are much too subtle or complex to be notated in any simple or useful way - by any notation system. Only careful listening, practice and experience can attune musicians to these subtleties. Much of the beauty of Indian Classical music also comes from the artist's ability to deliver inspired improvisations during a performance.  A reliance on a fixed score could hobble and constrain the artist and rob the music of its organic dynamism.  Learning Indian Classical music is largely about how to learning to compose music while simultaneously performing it. This is very different than the European Classical approach, where an artist practices to perform an unchanging musical score, and is never involved in its composition. When Sargam notation is used, it is thus only ever as a memory aid, and then usually just to jot down key recurring melodies.

That's the conventional place of notation in Indian classical music. But form the point of view of a student who is just starting to learn, the use some kind of notation system is pretty much essential. Casual students who are not deeply involved in the musical tradition, who don't come from a professional musical family, or who don't have regular access to a teacher, would find learning much more difficult without it. Notation can help students quickly grasp musical structures and patterns, give them a fixed reference to help internalize melodies, and allow for self-study if a teacher is not available. And even though improvisation is a key aspect of the sitarist’s art, it's also an advanced one. The first few years of a student’s learning will always be from a fixed score of some kind, even if that score is just transmitted orally and memorized by students during lessons. Notation is a great launching pad on which to build improvisational skills gradually.
Digital Sargam

This brings me to the reasons why I've written this article. As long-term student of the sitar, I've spent a great deal of time working with traditional Sargam notation. It’s been very helpful, but suffers from a few big limitations:

•	There’s no standardized notation system. 
•	It can’t accurately describe many of the complexities of rhythm and melodic phrasing.
•	It can’t be written on a single line of text using a standard computer without specialized fonts or software. 
•	It can’t be notated using a mobile device, like a phone or tablet.
•	It can’t describe how notes should be physically played or phrased on the sitar.

To solve these problems I’ve devised a modern system of sargam notation called Digital Sargam 1.0.   The “1.0” indicates that this is a first draft. I intend to update this framework as I encounter new use cases that it needs to solve. The overriding principles guiding the design of Digital Sargam have been simplicity, clarity and helpfulness. 

A student of the sitar can learn Digital Sargam within a few minutes. It can be used to quickly and easily notate simple phrases and compositions using a simple text editor on a computer, a mobile device, or a pencil and paper. It’s also capable of describing very complex compositions and subtle phrasings, as well as indicating fingering, fret positions for mir (string bending) and the right hand Da and Ra strokes that should be used. And because it’s a standardized system, students and teachers can freely share written scores with confidence that the music will be understood and played accurately.

So how do you read and write Digital Sargam notation? Let’s find out.

### Notes and octaves

To show that a note belongs to the higher octave, follow it with a single quotation mark.

````
S’
````

To show that it belongs to a lower octave, follow it with a comma.

````
S,
````

Once you’ve indicated the new octave, you don’t need to continue to do so for successive note. For example, take a look at the following phrase, which starts in the middle octave and ends in the upper octave.

````
S R G m P D N S’ R’ G’
````

<audio controls><source src="audio/6.mp3"></audio>

The single quote marks after S’ R’ G’ indicate that those notes belong to the higher octave. However, in this case those marks are entirely optional. Whenever you encounter a sequential series of notes like this, it’s implied that the phrase will continue into the upper octave. That means you can write the same phrase like this:

````
S R G m P D N S R G
````

There are no quote marks after the final S R G, but because they follow the natural progression of the phrase from the middle octave, it’s understood that they belong to the upper octave. This makes it quicker to write, and avoids cluttering the score with lots of redundant octave marks.

If you prefer, you can explicitly indicate that the phrase has entered the upper octave by just marking the first note of that octave with a single quote.

````
S R G m P D N S’ R G
````

The final S R and G belong to the upper octave, but only the first S is explicitly notated as such. This is a good compromise between clarity and efficiency. 

Here’s an example that describes a phrase that jumps from the middle octave, to the higher octave.

````
S R S S’ R S
````

<audio controls><source src="audio/7.mp3"></audio>

Here’s a phrase that starts on the low octave, jumps to the middle octave, and then jumps again to the high octave.

````
S, R S S’ R S S’ R S
````

<audio controls><source src="audio/8.mp3"></audio>

To show that a note is two octaves above the preceding note, use two single quote marks. The following phrase jumps from the low octave to the high octave.

````
S, R S S’’ R S
````

<audio controls><source src="audio/9.mp3"></audio>

Use two commas after a note to show a 2 octave drop.

The chikari strings (the sitar’s open drone strings) are indicated by a less than symbol.

````
<
````
<audio controls><source src="audio/10.mp3"></audio>

Here’s how to use it to write a simple jhalla pattern using this symbol.

````
S’<<< N<<< D<<< P<<< M<<< G<<< R<<< S<<<
````
<audio controls><source src="audio/11.mp3"></audio>

### Note durations

Blank spaces between notes are used to separate the beats that those notes fall on. For example, imagine that you’ve set your metronome to 50 bpm. In the following phrase, each note falls on a single tick of the metronome.

````
S R G m P D N S’
````
<audio controls><source src="audio/12.mp3"></audio>

Each note in the above phase occupies a whole beat. Spaces separate each beat.

For two notes per beat, group a pair of notes together, without a space between them. This is an example of the same phrase above played at double speed.

````
SR Gm PD NS’
````
<audio controls><source src="audio/13.mp3"></audio>

In the above phrase, each note has a duration of half a beat. The blank space between pairs of notes indicates a new beat.

Here’s how you’d write 4 notes per beat.

````
SRGm PDNS’
````
<audio controls><source src="audio/14.mp3"></audio>

Triplets are three notes that occupy the space of a single beat. They’re very common in Indian Classical music, and you can write them like this:

````
SRG mPD NS’R
````
<audio controls><source src="audio/15.mp3"></audio>

Here’s an example of how you can combine triplets with notes of standard duration.

````
SRGm PDN S’RGm
````
<audio controls><source src="audio/16.mp3"></audio>

The three notes in the middle, PDN, are the triplet, and occupy the duration of a single beat.

To extend the duration of a note, use a dash.

````
-
````

For example, here’s a phrase where each note has an equal value.

````
SRGmP
````
<audio controls><source src="audio/17.mp3"></audio>

Use a dash after each note to extend its value, so that each note is twice as long.

````
S-R-G-m-P-
````
<audio controls><source src="audio/18.mp3"></audio>

The duration value of the dash will be the same as the note that precedes it.

Use dashes to create rhythmic variety, like this:

````
S-RG-mP-DNS’
````
<audio controls><source src="audio/19.mp3"></audio>

Sometimes it’s helpful to use dashes to explicitly describe the length of notes. For example, here’s a simple 4 beat phrase. 

````
n, DD n S
````
<audio controls><source src="audio/20.mp3"></audio>

As you know, each space indicates a division between the beats. However, only the second beat contains two notes (DD). This could be confusing to read, so it might be clearer to write the phrase like this:

````
n,- DD n- S-
````

Even though the dashes are unnecessary, it makes it very clear what the duration of each note is. This is just a matter of style, so it’s up to you to decide how you prefer to write phrases like this.

You can also use a dash to indicate an entire empty beat.

````
S - R G - - m P
````
<audio controls><source src="audio/21.mp3"></audio>

In this example, each note occupies a full beat. Because you know that dashes have a duration that’s equal to the note that precedes it, each dash also occupies a full beat.
Taal divisions

Indian Classical music uses a system called taal to organize music into repeating rhythmic cycles. Here’s an example of a composition in Raag Kafi, set in teen taal, a common 16 beat rhythmic cycle. I’ve organized it using the two most important divisions in teen taal, the som (+) an the khali (0).

````
+
n, DD n S < S S nn
0
S g < R R gg mm
+
P - - D P mm g R 
0
g RR Gm Pm g- gR -R S
````
<audio controls><source src="audio/22.mp3"></audio>

The plus symbol (+) indicates the som (the first beat of the cycle.) The 0 symbol indicates the khali (the ninth beat.) You can see that a new line of notes starts with each division of the taal. This is important, because by vertically stacking divisions of even duration like this you can reveal patterns in the music. And, if you’re transcribing music, this helps you to make sure that your note durations work out to an even number for each division.

It’s up to you to decide which taal divisions you want to use to organize your music. Here’s an example of the same composition organized using all four of the traditional talis (claps) of teentaal: + 2 0 3.

````
+
n, DD n 
2
S < S S nn
0
S g < R 
3
R gg mm
+
P - - D 
2
P mm g R 
0
g RR Gm Pm 
3
g- gR -R S
````

Instead of the traditional divisions you can also divide each section according to its beat number, like this:

````
1
n, DD n S < S S nn
9
S g < R R gg mm
1
P - - D P mm g R 
9
g RR Gm Pm g- gR -R S
````

In this example, the + and 0 have been replaced by 1 and 9, which are the beat number values. Use whichever style you find more readable or understandable.

### Phrasing

Use a * symbol (asterisk) to highlight the beginning of a phrase that might be obscured by the beat and taal divisions. For example, here’s a common sequence of notes that contains 3 distinct phrases.

````
SRgSRgmSRgmPDnS’-
````
<audio controls><source src="audio/23.mp3"></audio>

There’s a clear pattern there when you listen to it, but you can’t see it in the notation and it’s very confusing to read. To clarify it, add an asterisk symbol at the beginning of each new phrase.

````
SRg*SRgm*SRgmPDnS’-
````

You can now easily see the pattern: 3-4-9. You can also clearly see that each new phrase starts on S.
Now let’s add spaces to give each note a duration of half a beat, and let’s start the phrase on the som.

````
+
SR g*S Rg m*S Rg mP Dn S’-
````

The beat divisions don’t match the phrase divisions, which is correct, but again, it’s difficult to read like this. To improve readability, let’s break each line at the beginning of every phrase, like this:

````
+
*SR g
*S Rg m
*S Rg mP Dn S’-
````

It’s now very easy to understand the structure of this phrase. (I added an optional extra asterisk to the first phrase so that it aligns neatly with the others.) In the Digital Sargam system you can break lines of notes in any way that clarifies the underlying structure of the music.

Here’s a longer, complete version of the entire phrase that spans 16 beats.

````
SR gS Rg mS Rg mP Dn S’- 
S’n DS’ nD PS’ nD Pm gR S-
````
<audio controls><source src="audio/24.mp3"></audio>

We can improve its readability by adding asterisks to mark the beginning of each phrase, and by adding taal divisions.

````
+
SR g*S Rg m*S Rg mP Dn S’-
0
S’n D*S’ nD P*S’ nD Pm gR S-
````

But it’s still a bit unclear, so let’s break each line at the beginning of a new phrase.

````
+
*SR g
*S Rg m
*S Rg mP Dn S’-
0
*S’n D
*S’ nD P
*S’ nD Pm gR S-
````

The shape and symmetry of the phrase is now obvious, and much easier to understand.

Align phrases like this in any way that makes the underlying patterns as clear to you as you need them to be.

### Repetition

If you want to repeat a phrase, surround it in square brackets and add a number that indicates the number of times it should be played. In the following example, the phrase inside the square brackets, S’NDPmGRS, is played twice.

````
[S’N DP mG RS]2
````
<audio controls><source src="audio/25.mp3"></audio>

The number 2 after the closing square brackets shows that the enclosed phrase should be played twice.

A tehai is a phrase repeated 3 times. Often the final note of the tehai will land on the first note of the rhythm cycle – the som. Here’s an example of how to write a tehai that starts on the 9th beat and ends on the som.

````
0
[SR Gm +P-]3
````
<audio controls><source src="audio/26.mp3"></audio>

The + symbol shows that the last note of the phrase, P, will land on the som on the third and final repetition.  Without this shortcut, you would have to write the tehai out like this:

````
0
SR Gm P- *SR Gm P- *SR Gm
+
P
````

### Da and Ra strokes


Sometimes you may need to clearly indicate which right hand strokes, Da or Ra, should be used to play notes. These are called bol (speaking) patterns.

Use a colon for Da.

````
:
````

Use a semicolon for Ra.

````
;
````

Place them in front of the notes that should be played with those strokes. Here’s an example of a phrase using a common bol pattern: da ra da da ra da da ra.

````
:S;R :G:m ;P:D :N;S
````
<audio controls><source src="audio/27.mp3"></audio>

Alternatively, if you find this too cluttered, write the bol pattern out separately directly after the notes of the phrase. Use “d” for the Da stroke and “r” for the Ra stoke like this:

````
SR Gm PD NS bol: drd*drd*dr
````

Add the asterisks to clarify phrasing if you need to.

### Krintan and Zamzama

Krintan is an ornamental technique where a note is played by pulling the second finger off the sitar’s main string while holding down the index finger on an adjacent lower fret. On Western string instruments, this is called a pull-off. You can indicate a krintan by surrounding the destination note in curly braces, like this.

````
{S}
````

There are two types of krintan. In the first type the starting note and the ending note have equal durations. You can write this type of krintan like this.

````
R{S}
````
<audio controls><source src="audio/28.mp3"></audio>

Here’s a phrase that uses this type of krintan.

````
PmGR{S}
````
<audio controls><source src="audio/29.mp3"></audio>

In this example you can hear that R and S have equal durations.

You can also play a krintan in an ascending note sequence by striking a fret with the second finger without playing a stroke. Western string instrument players call this a hammer-on. Notate it like this:

````
N,{S}
````
<audio controls><source src="audio/30.mp3"></audio>

In the second type of krintan, the starting note or notes are mere ornaments of the ending note. Their note duration is probably about 1/4 to 1/8th of the ending note’s value, but they’re not considered to have any real duration. This is the same as the Western musical ornamentation technique called acciaccatura (“crush”). So let’s call this a crushed krintan.

In the crushed krintan, the all the notes are surrounded by curly braces, but only the last note gets the full note duration. 

````
{RSNS}
````
<audio controls><source src="audio/31.mp3"></audio>

Here’s how to integrate this type of krintan into a longer phrase.

````
P m {mGRG} R S
````
<audio controls><source src="audio/32.mp3"></audio>

In this example you can hear that the krintan’s last note, G, is held for the full note duration, while the preceding notes, mGR, are scarcely perceptible. Whether those preceding notes fall directly before or after the beat is matter of personal playing preference and aesthetic choice.

You can notate a related technique called zamzama in the same way. Zamzama is just a 2 note crushed krintan. It’s a fast hammer-on, played twice in a row. Notate it like this:

````
{mP}{mP}
````
<audio controls><source src="audio/33.mp3"></audio>

Here’s a phrase that uses zamzama.

````
{mP}{mP} mG RG S-
````
<audio controls><source src="audio/34.mp3"></audio>

(In case you’re wondering, the word zamzama is onomatopoeia for the sound of a canon firing. In Lahore, in present day Pakistan, there is a famous historical canon called the Zamzama, which makes an illustrious literary appearance in the first sentence of Rudyard Kipling’s novel Kim: “He sat, in defiance of municipal orders, astride the gun Zam-Zammah...”)


### Mir (Meend) – String bending

Mir is the sitar’s famous and unique string bending technique. (It’s usually spelled meend, but pronounced mir.)  To notate a bend from a lower note to a higher note, use parentheses, like this this:

````
S(RG)
````
<audio controls><source src="audio/35.mp3"></audio>

The bend starts on the S fret, and R and G are voiced by bending the string.

To start the bend at a higher note, and bend down to a lower note, first surround the lowest note of the bend in parentheses. This will be the fret on which the bend happens.

````
(S)(GRS)
````
<audio controls><source src="audio/36.mp3"></audio>

In this example only the notes G R S are heard. The first note in parentheses, (S), just indicates the fret position from which the mir should be played.

It’s usually not necessary to explicitly indicate whether or not the right hand should strike the string during mir, because this is guided by common playing conventions that most sitar players follow according to the gharana (stylistic school) in which they’ve learnt. For example, during slow movements, like alap, only the first note of the mir sequence is usually struck using a Da stroke. During fast movements, like taans, all notes are usually played with Da Ra strokes. However, this may not always be the case, so it might be useful to indicate whether any notes within the mir sequence should be stuck.

In the following example, the G note within the mir sequence is struck using a Ra stroke, as indicated by the semicolon that precedes it. 

````
R(Gm;Gm-)
````
<audio controls><source src="audio/37.mp3"></audio>

In this example, the first note, R, is struck with the Da stroke, and the G note in the middle of the sequence is struck with the Ra stroke.

You will have to decide whether you need to explicitly notate Da or Ra strokes like this within a mir sequence, depending on the level of detail your composition requires.

### Slide

Use a tilde symbol to show that the player should produce an audible slide between notes.

````
S~P
````
<audio controls><source src="audio/38.mp3"></audio>

In this example only the S note is struck, and the index finger of the left hand audibly slides to the P fret.

### Flat stroke

A special sitar technique is to strike the string with a flattened Ra stroke so that the mizrab (wire plectrum) hits the tarraf (sympathetic) strings. Indicate this with the “cat’s ear” symbol: ^.  Here’s how to use it in a phrase in which the last note, P, is played with a flat stroke.

````
SRGm^P
````
<audio controls><source src="audio/39.mp3"></audio>

An alternative way of playing a flat stroke is to flick the bottom tarraf strings with the pinky finger of the left hand while simultaneously striking the main note with the right hand.

### Fingering

In some cases you may want to indicate which fingers of the left hand to use to play a note or sequence of notes. Precede each note with 1, 2 or 3: 1 for the index finger, 2 for the middle finger, and 3 for the ring finger.

Here’s how to notate that the mir, starting from the R fret, should be played with the second finger of the left hand.

````
2R(Gm) 
````

### Writing complex compositions

You can use the Digital Sargam notation system to write or transcribe any sitar music, no matter how complex. Here’s a very advanced, example of a complete vilambit (slow tempo) composition in Raag Kafi that uses most of the elements of this notation system. This is an extreme case; most compositions will be far simpler than this. It would never be recommended that you learn a composition of this complexity directly from the notation. Instead, learn the composition by carefully listening to an audio or video recording of it, and use the notation simply as a memory aid. It’s a lot easier that way.


Asthaiy (main, middle octave, section of the gat)

````
12
P(Dn;Dn--:n D-P-----)
13
m{(P)(DP)}P {mgRg}R n,-{SR}-
1
S S S (D)(SnD-)n- 
5
S {Rg}-R- -Rm P(Dn;Dn--:n 
13
D-P-----) m{(P)DP}P {mgRg}R
12
Gat
````

Antara (upper octave section of the gat)

````
13
{Pm} PP (D)(nD-) nR' 
1
S S S Dn
5
(sRg-r-g- rS) {Sn}D P 
3
m{(P)(DP)}P {mgRg}R n,RS-
12
Gat
````
<audio controls><source src="audio/40.mp3"></audio>

The recording starts on the first beat of the teentaal cycle so you can clearly hear where the composition begins on the 12th. 

In the recording you’ll hear that between notes or phrases are “fillers” made by strumming the chikari strings and striking the jora string with the right hand. When and how to play these fillers is an aesthetic decision that’s left to the sitarist, so it’s not usual to notate these.  However, you could easily do so by using the symbols for the low Sa jora string and the chikari strings.

````
S, < 
````

You can also use Digital Sargam to write alap phrases. In that case, note durations and timings will simply be understood to be approximate and paced with feeling.

### Learning Digital Sargam

The best way to learn Digital Sargam is just to start writing it. Begin with simple compositions that you know well, and use the examples in this document as a guide to writing them. 

*This work, including the audio examples, is entirely license and copyright free. Distribute it, re-publish it, re-word it, re-write it, and improve it at your pleasure. It was funded in part with the assistance of the [Shastri Indo-Canadian Institute](http://www.sici.org). Many of the notation examples, including the traditional Kafi compositions, are from Sahana Banerjee, a leading sitarist of the Senia-Rampur Gharana (school) of Indian Classical Music.*

To contribute to this ongoing work, please visit: http://www.github.com/sargam/digital.


