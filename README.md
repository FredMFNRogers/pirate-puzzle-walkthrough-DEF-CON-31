# Pirate puzzle 31

This puzzle is not for the faint of heart. It’s loaded with secrets and obscure references. And trains. Everything is obvious, but only in hindsight. We, the Salty Seven, have put this guide together to get you through the rough times. However, we dare you not to peek until you complete the puzzle.

[Start the puzzle here](https://dc31.whiskeypirates.org/) and heed the warnings. In particular, “if an answer isn't obvious, it's probably not the answer.”

Hope this helps! Sincerely, The Salty Seven:
catladytaylor, feath3rz, B!gD@wg, P4cketDefense, fred rogers, Bokonon, and heckseven

## 1. The pirate puzzle portal

What a perfect website. Amazing gifs and a web ring to join. Before getting started, it might help to peek at the code - in particular, take a look at this comment:
  

```html
<!-- to make it obvious:  if you're smart and you're reading this, you will *need* either the DVD iso and  -->
<!-- photo, or the physical disc to complete the puzzles. a pirate puzzle or wp puzzle BADGE may be needed -->
<!-- to solve this puzzle. if you don't have our puzzle badge, you can use the free online badge emulator. -->
<!-- unzip the zip file located in the "bemu" folder on the DISC. the thing you'll need to unzip this file -->
<!-- is the single long werd piracy lives forever without any spaces for the link to the emulator website. -->
```

Nice. Use the access code provided in the form to get a link to download the disc:

`disc`: [PIRATEPUZZLE.iso](https://puzzle31.whiskeypirates.com/wp_dvd_final_v004.iso)
## 2. The disc

Once downloaded, mount the disc and familiarize yourself with the contents. There are plenty of things going on. Before getting too carried away, extract the contents of `bemu.zip`.

```sh
$ 7z x bemu.zip
```

In the extracted `bemu.txt` you will find links to the [emulator](https://dc31.whiskeypirates.com/pp_badge_emu) along with further instructions on how to proceed with the puzzle.

Then, take a look at the disc's `readme.txt`. Inside are more details about the puzzle including how to use the phone system. Definitely give it a call.

Use the code, `puzl`, from `readme.txt` to start the puzzle.

`puzl`: [access granted](https://puzzle31.whiskeypirates.com/stage1/)
## 3. Stage 1

The three images are from a show called Robbie Rotten and are all called `a.gif`. This indicates a ROT3 cipher shown below:

```
zrzwklvzdvhdvbxvhwkhdffhvvfrghkbaz
```

When decoded:

```
wowthiswaseasyusetheaccesscodehyxw
```

`hyxw`: [just warming up](https://puzzle31.whiskeypirates.com/zyxlolno/)

**Note:** The URL implies the existence of other stages. [Stage 2](https://puzzle31.whiskeypirates.com/stage2/) is a trap. It is not a puzzle. Feel free to try to solve it.
## 4. This is just a warmup

There is an image of someone working out and several puns about resistance. If you look closely, you can see the resistance bands could be resistor bands.

Related inputs provide additional clues:

```
watt:
no, not even a watt. at DC31's 120V,
it's roughly three quarters of a watt.
the answer isn't a random word guys.
look closer at the picture, the title, the obvious hints…
ohms: you're getting the hint. now put it all together.
```

Use a resistance calculator and select the colors from the resistance bands. It should result in a 20k ohms resistor. The ohm symbol didn't work, but `o` did resulting in an access code of `20ko`.

`20ko`: [bam](https://puzzle31.whiskeypirates.com/xbambam/)
## 5. Bam

An image of bambam from the Flinstones with an `@` symbol on the bat. The image is accompanied by another cipher:

```
gsvozhgxlwvrhirtsg
yfgrhgsvvmwrmhrtsg
wruurxfogbrhizrhvw
drgsgsvmvdxlwvgzaw
```

The name of the cipher is related to bambam's bat. It's the atbash cipher. This decodes to:

```
thelastcodeisright
butistheendinsight
difficultyisraised
withthenewcodetazd
```

Using the code, `tazd` will start training.

```
tazd:
	there be a pattern, color a designation;
	the side holds A seCret... so I've heard.
	long rails and brands, loud horns on silver engines;
	each one will be counted... that's for sure.
	big kars on the traks, nostalgia for some of us;
	these days personal transport preferred.
	obvious coding, even if barley misplaced;
	deleet to make an unintelligible word.
```
## 6. Training

On the DVD, there are train images in `images/trains`. It took a long time to find, but there was a specific image with something funky. The train in `31.jpg` has codes on the door. After some searching, we found those codes are [KarTrak codes](https://en.wikipedia.org/wiki/KarTrak#/media/File:KarTrak_ACI_codes.svg) which are effectively old school bar codes.

![image](https://upload.wikimedia.org/wikipedia/commons/thumb/e/eb/KarTrak_ACI_codes.svg/800px-KarTrak_ACI_codes.svg.png)

The KarTrak code decodes to `3057`.

```
3057:
	the most powerful
	too leet for me
```

Well if it’s too leet, time to try the de-1337ing it into `eost`:

```
eost:
	the badge cargo is delivered.
	the secrets of our rulers?
	it's... not really a secret
```

Note: `not really a secret` has zero width spaces. Maybe this is a clue... ;)
## 7. Lizard people

The previous clue mentions rulers. On the DVD, in `/badge`, there is an encrypted archive called `ruler.zip`. The clue above hints at the password, `notreallyasecret`. This will unzip the document revealing a new file called `ruler.htm`. Open it up in a browser.

You'll see an interesting image that looks like the characters `7z` and some clues below it. Either save the image or open it in a new tab. It's transparent and, in the image, there is a hidden message not visible on a dark background. It says, "BOMBTHELIZARDS".

Below the image is the text:

```
THE LIZARDS HAVE THE TECHNOLOGY
THEY ARE ALWAYS WATCHING
DON'T THINK TWICE
```

Funny enough, there is an archive called `tech.7z` in the same directory.

`7z x tech.7z` with the password `BOMBTHELIZARDS` results in an error:

```
Path = tech.7z
Type = 7z
Physical Size = 17730
Headers Size = 226
Method = 04F71106 7zAES
Solid = -
Blocks = 1

ERROR: Unsupported Method : thebomb.jpg
```

The page title hints that maybe the archive isn't 7zip:

```html
<title>stuffed with lizard technology</title>
```

If you search for `lizard compression` or some of the details in the error message, you'll learn that there is such a thing as lizard compression. I had to pop over to Windows and install `7Zip ZS` to unzip `tech.7z`.

Once you have the right password and the right software, extract an image of a bomb. `thebomb.jpg` has a bunch of wires drawn on it with "Don't Cut the Wrong Wire" written on it along with "Countdown 8". The wires correspond to badge wiring. Definitely try this on a puzzle badge if you have one. It’s cool af. When you input a code, the badge will flash binary at you that translates to a string.

```
Input: 23018647
01000100
01000110
01010101
00110101
Translates: "DFU5"
```

There are two other messages possible when wiring this up:

```
Input: 23518647
01000001
01110010
01101101
01100101
01100100
00101110
00000000
Translates: "Armed."
  
Input: 03518647
01000010
01001111
01001111
01001101
Translates: "BOOM"
```

Okay, with the bomb defused, we get the code, `DFU5`:

`DFU5`: [sugar rush](https://puzzle31.whiskeypirates.com/hacker0s/)
## 8. Hacker Os

Inspect the html to find a clue:

```html
<!-- but the real world may not accept you unless you hide your leet. -->
<!-- does not mean you aren't a hacker. doesn't mean you aren't leet. -->
<!-- just sometimes you have to blend in with the normies to be leet. -->
```

The text on the page is really all you need for this one:

```
all the skiddies are dropping their O's!
start your quest off right with hacker 0's!

make a difference and 1337ify your life!
call now to order: 91258-27788
```

When looking at the “Call now to order” line, it is obvious that it is not a proper phone number so the most straight forward answer is to 

Do the math: 91258 - 27788 = 63470

The beginning of the text of the clue tells you that everyone is dropping their “o’s” so that leaves you with 6347.

The inspected html tells you that sometimes you have to blend in and hide your l33tness, so if you de1337ify 6347, you get a few options to use.  6 can be g or b, 3 is almost always e, 4 is a and 7 can be l, t, or y by itself so there are a few iterations, but when you view it as a word you get the code `beat`.

```
beat:
	the brands, the lies, the deceit
	made of corn, rice and wheat
	hiding in plain sight
	are five things that might
	blow you out of your seat

	the cereal is telling you lies
	remove the ones with the eyes
	the one that remains
	will destroy your brains
	when its name rotates its disguise
```

This clearly references the `images/cereal` directory. There are five images with four letter names. Four of those images have the letter `i`. If we remove those, we are left with `bomb.jpg`. In that image is a cereal box with the Joker on it and a bomb in the bottom right corner. The bomb in the corner is five sticks of dynamite that "might blow you out of your seat."

If we take the name of that image, `bomb` and rotate it, we get `qwoq`. 

```
qwoq:
	it looks like you believe in the conspiracy
	  
	moving forward is easy:
	   use the access code made of the last four characters
	     of the confirmation number of the prior access code
	  
	in order. nothing weird. no games.
	
	it's getting real.
```

The last four digits of the `beat` code are `34d4`.

`34d4`: [yup. it's real.](https://puzzle31.whiskeypirates.com/playtime/)
## 9. Final

It's a playfair cipher. The clues on the word search indicate you need the first letter of the hackers from the list. The list included characters from the movie, Hackers. Fill in the playfair key with those letters (Z from Zero Cool, A from Acide Burn, etc) and then fill in the rest with missing letters in ascending order essentially following the instructions on the word search.

This resulted in the code: `ZAPCLJBDEFGHIKMNOQRSTUVWX` to decode the following text:

```
AVLTAZDKRXQOARTNOCXNUGKWDKNQRJDMOZPFSUQSZOIQUNCDONUKJRPMNXJRHBERUCQEOLPRVHWKGRRUCFJIJWKBQJKEQBJWKBRFHLWRGQMNQODQOCWJIQRLQOEKUGFRKEWKWJRZQBFEPQQMFABWAQONWOBLEKSBUGKWUAQJMQEFPKAIKWFEOBPQTNZOKGPZAKKEMRXHDMQJQOJKWKWFOQOEAXJRPCMKRTGVKOFEGQICJRQSLHCORKWCQKWJQOGVTUKBIQRLRFEWJWURQENSDWBCCFEVGVIHSQVAOZKFZOBPXOKWOBQJCFPZNQHLWRQOUGFJPLDCCOAKKFTZPZLFARSJKQHLVGQOTSXHDFSNGQUGJWQKPZOFVUOQPLWLFRLXAREFNXWOQGQZPCKWZOEVQKVGTNGQNXOWKFTZTURBGVKBQCKQZUFRWEQOQSWNWBIQWKZWZUEFELQOHAVGJSNUGQZPQXJKLOKWXHRHUGJRXOKWHXNXRFQJAINUSUSBHUUGCPCDOCQJGQMKTNEFPQEKUNXOGQCQQPZUFKFRLXZHBRWKHLMPUGTXKCMPLFKFWFXNSUQOa
```

This results in:

```
PUZXZLEISWONCONGRATSTHEREISONEFINALDOXORANDITOPENSWHENLISTENBACKWARDSACQUIREKNOWLEDGETHENDECODETHESEMARKINGSONPIRATEDISCONCETHESECRETENCODEDVISIBLEUPONSURFACEOFTHEROUNDISDECIPHEREDHAVINGANIMALCHECKSUMFINDONEGREXENORBLUENAPKINWITHREDINKPENORAMARKERWRITEONITXTHEDISCSECRETWORDSREVEALEDWITHGROUPNAMEANDAUSERHANDLEALSOMARKONTHEFACEPARCHMENTALXLCONFIRMATIONXNUMBERSINTHETRIALSBUTNOACXCESXSCODESTURNINPAPERANDWRITINGINSTRUMENTXTOEITHERPIRATESRCONORTRUEDIRECTATDEFCONBUTIFNOTINLASVEGASERUMOKTHENUSERMUSTSENDPHOTOXOFBOTHPAPERANDINKINGDEVICETOUSINPRIVATEMESXSAGEOREMAILTHXWEWILXLMEXETSOXONLU
```

Playfair doesn’t like two repeating letters so there are extra X’s everywhere. Just delete them, add some spaces and get:

```
PUZZLE IS WON CONGRATS
THERE IS ONE FINAL DOOR AND IT OPENS WHEN LISTEN BACKWARDS
ACQUIRE KNOWLEDGE THEN DECODE THESE MARKINGS ON PIRATE DISC
ONCE THE SECRET ENCODED VISIBLE UPON SURFACE OF THE ROUND IS DECIPHERED HAVING ANIMAL VALIDATION.

FIND ONE GREEN OR BLUE NAPKIN WITH RED INK PEN OR A MARKER WRITE ON IT THE DISC SECRET WORDS REVEALED WITH GROUP NAME AND A USER HANDLE ALSO MARK ON THE FACE PARCHMENT ALL CONFIRMATION NUMBERS IN THE TRIALS BUT NO ACCESS CODES TURN IN PAPER AND WRITING INSTRUMENT TO EITHER PIRATES R CON OR TRUE DIRECT AT DEFCON BUT IF NOT IN LAS VEGAS ERUMOK THEN USER MUST SEND PHOTO OF BOTH PAPER AND INKING DEVICE TO US IN PRIVATE MESSAGE OR EMAIL THWE WILL MEET SOON LU
```

### 9A. The final door

Based on the previous clues, the songs in `tunes/daos` folder were reversed and identified as System of a Down tracks (daos is SoaD mirrored).

One of these is the four letter song ATWA

If you enter `ATWA` in the portal:

```
PUZL edoc ssecca eht retne eerga uoy fi
uoy ro ylevisulcxe si niahc siht fo dne eht
eno suoivbo siht ylno rof tpecxe...
derorrimnu deretne eb lliw sedoc ssecca
smlaer rehto eht ot ylppa ton od dna
noitalosi ni era mlaer siht fo selur
deppilf ro derorrim neht sdrawkcab ton fi
sdrawkcab si niahc siht ni gnihtyreve
mlaer rorrim eht gniretne era uoy
```

Which reversed is:

```
you are entering the mirror realm
everything in this chain is backwards
if not backwards then mirrored or flipped
rules of this realm are in isolation
and do not apply to the other realms
access codes will be entered unmirrored
...except for only this obvious one
the end of this chain is exclusively or you
if you agree enter the access code LZUP
```

Entering in the code LZUP yields this [puztile.png](https://puzzle31.whiskeypirates.com/img/puztile.png) surrounded by this hidden text:

```
ereht ot og lliw
the secondary tool is your brain bmob eht si emag isht
ereh morf semoc tahw
```

translating to:

```
will go to there
the secondary tool is your brain
this game is the bomb
what comes from here
```

On the image is a domino. The left half has four dots: top left is red, bottom right is green, rest are black. On the right half of the tile is two dots: top green, bottom red.

```
_____________________
|                   |
| R B - - | G - - - |
|         |         |
| B G - - | - - - R |
|___________________|

```

If you mirror the domino and connect the dots with their corresponding color, you will realize this is hinting at using the puzzle badge. This results in the following input for the badge: `10000052`. In other words, the red dot in the top left above is actually output 1 on the badge. The red dot on the bottom right above is the input number 8.

Input `10000052` into the badge to get the following results:

```
01001110
01011001
01010010
01000100
Translates: `NYRD`
```

`nyrd`: Reveals the following image and a new challenge:
### 9B. The Mirror of Denial  

There is an image of Bart and Lisa Simpson that says “LOOK! THE MIRROR OF DENIAL!” and a cipher that looks very much like a polybius cipher. There is an image of an arcade in `images/webjunk/`. On one of the arcade cabinets is a polybius grid. 

![mirror of denial](https://puzzle31.whiskeypirates.com/img/dmirror.jpg)

```
51134212 1243 413351 3451134244535124 513244 32444225 13115141 4344 451125 513343 33113244 51244323 3442 5124513244 334342445343 44341113 513244 3442 34423244 33254341 2233424322 3442 4442
```

Reverses to:
  
```
2444 2443 2234243322 14345233 44232443 2443 442315 31114344 343544243433 4423154215 2443 32344215 44231133 343315 521154 4434 14151131 52244423 442315 4215354424311543 153314 3421 21243115
```

Which, when fed into the polybius square, yields:

```  
IT IS GOING DOWN THIS IS THE LAST OPTION THERE IS MORE THAN ONE WAY TO DEAL WITH THE REPTILES ENDOFFILE
```

Additionally, there is a comment in the html of this page with more ciphertext:

``` html
<!--
51444451544332
13423433515144
24423244513244
12434133515132
44441152434313
ot deen ll'uoy
-->
```

Reverse the html comment and put it into a polybius square to get: `LOOK AT THE END OF THE THIRTEEN SILHOUETTE`

Perhaps it’s time to take a closer look at the image from `ruler.htm`.
### 9C. Maybe think twice

Let’s look at that lizard image. It has an outline of thirteen lizards which seems to match the above clue.

First, inspect the code. You'll see the image is base64 encoded. At the end of the image, you'll spot something that doesn't look like it belongs. If you decode everything after the `/`, you will get another clue: `maybethinktwiceaboutthebomb`. Oh hey! Another password. Perhaps to `watcher.7z`?

In the `/badge` directory, this is another archive called `watcher.7z`. Unzip it using the password `maybethinktwiceaboutthebomb` to get a new image called `reality.png`. Looking at the image, it says:

```
THE
BOMB
IS THE
ONLY WAY
```

That doesn’t mean much yet. Let’s go deeper. Open the image in a text editor (or just run `strings reality.jpg`) and scroll to the bottom to reveal another clue:

```
you are making the right choice if you proceed normally. however, your choice is not mutually exclusive. to complete your journey, you'll need to proceed this way too. you are so close. here is how to make the key you will need. it's easy and straightforward, even if it sounds complicated. there are no tricks. simply concatenate the last ten characters of the output of the access code DONE with the confirmation number given when you are ready to play nice. this will be the hex key you need. congratuations in advance.
```

Nice! We are making progress!

```
done:
	168ddb050df891f437f5e95a36ffb30c
	92808229f8274975f4c381798e0bf47e
```

101337 is the confirmation number of the puzzle in Challenge 11. Concatenating that with the last 10 characters of `done` yields `798e0bf47e101337`
## 10. The finale

Just to refresh your memory, the first part of the output of the word search cipher:

```
PUZZLE IS WON CONGRATS
THERE IS ONE FINAL DOOR AND IT OPENS WHEN LISTEN BACKWARDS
ACQUIRE KNOWLEDGE THEN DECODE THESE MARKINGS ON PIRATE DISC
ONCE THE SECRET ENCODED VISIBLE UPON SURFACE OF THE ROUND IS DECIPHERED HAVING ANIMAL VALIDATION.
```

We now have a key. Let’s look at the code. On the surface of the disc are 16 bits. There is no indicator which bit is first, so it is best to rotate the string to get every variation:

```
B5 2C 42 5C 63 29 CB 4C B8 3B 57 52 79 3D CF 5B
2C 42 5C 63 29 CB 4C B8 3B 57 52 79 3D CF 5B B5 
42 5C 63 29 CB 4C B8 3B 57 52 79 3D CF 5B B5 2C 
5C 63 29 CB 4C B8 3B 57 52 79 3D CF 5B B5 2C 42 
63 29 CB 4C B8 3B 57 52 79 3D CF 5B B5 2C 42 5C 
29 CB 4C B8 3B 57 52 79 3D CF 5B B5 2C 42 5C 63 
CB 4C B8 3B 57 52 79 3D CF 5B B5 2C 42 5C 63 29 
4C B8 3B 57 52 79 3D CF 5B B5 2C 42 5C 63 29 CB 
B8 3B 57 52 79 3D CF 5B B5 2C 42 5C 63 29 CB 4C 
3B 57 52 79 3D CF 5B B5 2C 42 5C 63 29 CB 4C B8 
57 52 79 3D CF 5B B5 2C 42 5C 63 29 CB 4C B8 3B 
52 79 3D CF 5B B5 2C 42 5C 63 29 CB 4C B8 3B 57 
79 3D CF 5B B5 2C 42 5C 63 29 CB 4C B8 3B 57 52
3D CF 5B B5 2C 42 5C 63 29 CB 4C B8 3B 57 52 79 
CF 5B B5 2C 42 5C 63 29 CB 4C B8 3B 57 52 79 3D 
5B B5 2C 42 5C 63 29 CB 4C B8 3B 57 52 79 3D CF 
```

Reading the text hidden in `reality.png`, we got the impression that we should use an XOR operation to decode the cipher using the key `798e0bf47e101337`.

Side note: Most of us were stuck here for weeks even though we all came to the same conclusion rather quickly. We were using Cyberchef to try to decode the cipher, but didn’t realize we needed to use the `From hex` module in Cyberchef before using the XOR operation. We tried MANY other things. Conspiracies were born. Conspiracies were killed. Anyhoo..

When XORing the entire set of rotated bits, we get mostly junk, but a single line stands out:

```
PEGLEGANDAPARROT
```

It translated from this particular rotation of the bits from the disc:

```
29 CB 4C B8 3B 57 52 79 3D CF 5B B5 2C 42 5C 63
```

Hell yes. We did it! Now, for the second part of the word search cipher:

```
FIND ONE GREEN OR BLUE NAPKIN WITH RED INK PEN OR A MARKER WRITE ON IT THE DISC SECRET WORDS REVEALED WITH GROUP NAME AND A USER HANDLE ALSO MARK ON THE FACE PARCHMENT ALL CONFIRMATION NUMBERS IN THE TRIALS BUT NO ACCESS CODES TURN IN PAPER AND WRITING INSTRUMENT TO EITHER PIRATES R CON OR TRUE DIRECT AT DEFCON BUT IF NOT IN LAS VEGAS ERUMOK THEN USER MUST SEND PHOTO OF BOTH PAPER AND INKING DEVICE TO US IN PRIVATE MESSAGE OR EMAIL THWE WILL MEET SOON LU
```

We scrounged up a blue napkin, a red dry erase marker, and followed the instructions:

![[theSaltySeven.jpg]]
## 11. Unsolved mysteries

There are apparently two unsolved bonus puzzles left. One likely involves `shortone.7z` and the other is... well... a mystery. Let us know if you figure them out!
## Confirmation codes:

```
ea94af
5ddf43
6ee43b
4a3ef5
d7222a
66dfb4
14ca8c
c734d4
532df2
101337
356ffc
4c5c83
9511f6
```
## Bonus codes

```
1337: y35, w3 kn0w w3 4r3 =)
hack: hack the planet
help: no
fuck: me silly
shit: sorry, I am a puzzle. I cannot defecate.
h8rz: we got the treasure (some images), but you do not
bomb: boom goes the conspiracy
evil: evil conspiracies
boom: lol, you died
know: you never think you know
corn: part of a balanced breakfast conspiracy
rice: part of a balanced breakfast conspiracy
capn: video (NEED TO WATCH)
boob: (.)(.)
poop: 💩
rofl:
	you think you're fucking clever. no.
nice try though. lmao.
blue:
	colors? what about colors?
	this is not how you would cut a color...
	(note: bruteforcing will never solve this puzzle.)
	(answers are mega obvious when you see them.)
wire:
	wire messenger is superior to signal
	pirates use wire, you should too
game: you lost the
bill:
	I'm just a bill
	on conspiracy hill
trix:
	trix are for kids
	a conspiracy to infiltrate their minds
120v:  
	why would this be an access code?
	look closer for something obvious, not every 4 letter word you see.
true:
	the whiskey pirates puzzle for defcon 31
	
	credits
	
	concept by rCON
	website and backend code by true
	puzzles by rCON and true
	puzzles pieced together by true
	badge design and code by true
	badge assembly by rCON and true
	disc mastering, disc concept by true
	art resources by random internet searches
	art modified by rCON and original work by true
	
	tested by anonymous testers. you know who you are
	
	thanks for supporting our work
	don't overthink shit and you'll do fine
	hope you have fun
rcon:
	the whiskey pirates puzzle for defcon 31
	
	credits
	
	concept by rCON
	website and backend code by true
	puzzles by rCON and true
	puzzles pieced together by true
	badge design and code by true
	badge assembly by rCON and true
	disc mastering, disc concept by true
	art resources by random internet searches
	art modified by rCON and original work by true
	
	tested by anonymous testers. you know who you are
	
	thanks for supporting our work
	don't overthink shit and you'll do fine
	hope you have fun
```