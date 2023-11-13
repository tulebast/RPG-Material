Integrating the Fate Font into your website
So you don’t want to go without the Fate dice symbols for your article on your Website?
Integrating the Fate webfont into your website is not a big deal, thanks to Jörn Heimeshoff, who has coded also the german online Reference for Fate Acclerated and Fate Core

Integrating the Fate Font into your website
To start, you need the font and some files you put into the same layer of your server as the CSS file. (If you use WordPress, simply put them into the theme’s root.)
Fate WebfontFate Webfont
Fate_Webfont.zip
Version: 1.0
19 KiB
804 Downloads
DETAILS

Now you integrate the following code snippet into the CSS file of your website or e.g. your worpress theme.
1
2
3
4
5
6
7
8
9
10
11
12
13
14
15
16
17
18
19
20
21
/* Fate Webfront einbinden */
@font-face {
font-family: 'fate';
src: url('fate_core_font-webfont.eot');
src: url('fate_core_font-webfont.eot?#iefix') format('embedded-opentype'),
url('fate_core_font-webfont.woff') format('woff'),
url('fate_core_font-webfont.ttf') format('truetype'),
url('fate_core_font-webfont.svg#fate_core_glyphsregular') format('svg');
font-weight: normal;
font-style: normal;
}
span.fate_font {
font-family: "fate";
font-weight: normal;
-webkit-font-smoothing: antialiased;
font-smoothing: antialiased;
}
span.fate_font.big {
font-size: 2em;
line-height: 1.2em;
}
<h1>The Licence Issue</h1>
As a next step, your should put this comment into the footer or the sidebar of your page:

The Fate Core font is © Evil Hat Productions, LLC and is used with permission.
The Four Actions icons were designed by Jeremy Keller.

<h1>Using the font:</h1>
After that use the span-tag to format your text:

Examples for Dice Rolls:
1
<span class="fate_font">-+0+</span>
leads to:
-+0+

Examples for the Action Symbols:
1
<span class="fate_font big">OCAD</span>
leads to OCAD

Overview:
Character	Html-Code		Outcome
Plus +	&#43;		+
Minus –	&#45;		-
Zero 0	&#48;		0


Action	Character		
Create Advantage	C		C
Overcome	O		O
Attack	A		A
Defend	D		D
Sample-Text:
Rolling the Dice
When you need to roll dice in Fate, pick up four Fate dice and roll them. When you read the dice, read every + as +1, every 0 as 0, and every – as –1. Add them all together. You’ll get a result from –4 to +4, most often between –2 and +2.

Here are some sample dice totals:

-+0+ = +1
+-00 = 0
+++- = +2
-000 = −1

The result on the dice isn’t your final total, however. If your character has a skill that’s appropriate to the action, you get to add your character’s rating in that skill to whatever you rolled.

So, once you’ve rolled the dice, how do you determine what a particular result means? Glad you asked.

Players, some of the things you’ll do in a Fate game require you to roll dice to see if your character succeeds or not. You will always roll the dice when you’re opposing another character with your efforts, or when there’s a significant obstacle in the way of your effort. Otherwise, just say what your character does and assume it happens.

OTo overcome an obstacle

CTo create or unlock an advantage for your character, in the form of an aspect you can use

ATo attack someone in a conflict

DTo defend yourself in a conflict

The Sourcecode:
1
2
3
4
5
6
7
8
9
10
11
<h4>Rolling the Dice</h4>
<p>When you need to roll dice in Fate, pick up four Fate dice and roll them. When you read the dice, read every <span class="fate_font">+</span> as +1, every <span class="fate_font">0</span> as 0, and every <span class="fate_font">-</span> as –1. Add them all together. You’ll get a result from –4 to +4, most often between –2 and +2.</p>
<p>Here are some sample dice totals:</p>
<p><span class="fate_font">-+0+</span> = +1<br /><span class="fate_font">+-00</span> =<br /><span class="fate_font">+++-</span> = +2<br /><span class="fate_font">-000</span> = −1</p>
<p>The result on the dice isn’t your final total, however. If your character has a skill that’s appropriate to the action, you get to add your character’s rating in that skill to whatever you rolled.</p>
<p>So, once you’ve rolled the dice, how do you determine what a particular result means? Glad you asked.</p>
Players, some of the things you’ll do in a Fate game require you to <strong>roll dice to see if your character succeeds or not. You will always roll the dice when you’re opposing another character with your efforts, or when there’s a significant obstacle in the way of your effort.</strong> Otherwise, just say what your character does and assume it happens.
<p><span class="fate_font big">O</span>To overcome an obstacle</p>
<p><span class="fate_font big">C</span>To create or unlock an advantage for your character, in the form of an aspect you can use</p>
<p><span class="fate_font big">A</span>To attack someone in a conflict</p>
<p><span class="fate_font big">D</span>To defend yourself in a conflict</p>
