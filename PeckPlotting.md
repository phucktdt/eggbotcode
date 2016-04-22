# Introduction #

I've been focusing my energies on the hard side, prepping for the Maker Faire in NY.  "Hard," as in diamond, glass, and constant annoying noise.  Maker Faires seem to provide the perfect impetus for me to really **use** my Eggbots, and see if I can reproducibly create high quality results.  Pre-San Mateo was eggs.  Pre-Detroit, drawing on glass bulbs.  For NY, I'm trying to see if I can take Windell's idea of using inexpensive ingredients (pager motor and diamond point) to engrave glass.  Blessedly (for her) my wife was out of town for the past four days, and I've been able to run experiments round the clock.  She returns tonight, and our rather tight space must return to its normal sanely organized and quiet state (very unlike NOW). Not real sure anyone will want to embark on his adventure, but while it's fresh in my mind, I wanted to document some of the trials I've made.

# Details #

Equipment to make "pecker" (sorry, but simply not resistible):
  * Diamond dresser nib--  McMaster 44045A61
  * Pager motor-- Radio Shack "micro vibration motor" 273-0107
  * dead Sharpie fine point pen
optional:
  * 1/8" ID, 3/8" OD shaft collar, aluminum-- McM 9946K41
  * 1/8" ID, 3/8" OD shaft collar, steel-- McM 9414T3


![http://eggbotcode.googlecode.com/svn/wiki/images/pecker.jpg](http://eggbotcode.googlecode.com/svn/wiki/images/pecker.jpg)

In Detroit, we tried our first peckplots, and I didn't realize at the time how lucky we were to have it work.  Lenore and Windell brought similar diamond points and Windell had one mounted in a 3/8" plastic dowel so it would fit into the penarm.  They had a variety of pager motors, and we used the largest-- but I'm not sure where it came from.  I had ordered some "smokey gray" xmas bulbs, 3.25" diam., for drawing on, and we tried these.  The tiny pits made by the point removed the opaque gray and allowed light to show through when we put some LED's in the bulbs-- very cool effect!  So my goal was to recreate this result.  First thing I did was to find some pager motors.  I got some small ones from Axman (wonderful local junk store in Mpls/St.Paul), but they didn't have much oomph.  I was surprised to find that RS carries one, and tried it-- much better!  It is rated at 3VDC, and I first ran it with two D-cells.  I then switched to a 5VDC regulated supply, with a 30 ohm 5W (overkill)resistor in line.  I see a voltage drop across it of 1.8V, so the motor is getting 3.2V.  A little Ohm's Lawing shows it draws ~60ma.  Although I expected it to die pretty quickly, since it is clearly not designed for continuous use, I am happy to report it is going strong after >100 hrs. In Detroit, we mounted the pager motor to the distal penarm, using a wire-tie and two of the slots that had been pre-cut.  I tried this approach first, but soon realized that 1) the motor works itself loose due to, um, vibration, and 2) it seemed like we want the vibratory energy to be as concentrated, up/dn, along the axis of the point.  I was also grappling with how to mount the 1/8" diam. diamond point shaft, when it hit me that using a Sharpie body might work.  Since I keep all the ones that get dried out (very useful, BTW, to check egg and penarm position), I sawed one in half, and easily removed the ink "sponge" (thankfully very dry and clean to work with).  I then pulled off the nib, and cut it off with a razor, just above the metal part.  I then drilled the remaining plastic cowling out to 1/8", and shoved the point's shaft in-- very nice, firm fit.  Next, I drilled a hole across the now empty body (15/64") to allow a (very) firm friction fit for the pager motor.  One of the nice aspects of this approach is that the "pecker" becomes just a specialized Sharpie that can be installed and removed as easily as a regular pen.

# Canvas #

Since the results in Detroit were so interesting, and I only had a few of the gray bulbs left, I ordered black bulbs (from http://ChristmasCentral.com/).  One type shiny, the other matte.    While I was waiting for them to arrive,
I created a TSP drawing of Mona (starting with a negative), and tried it on one of the remaining gray bulbs.

![http://eggbotcode.googlecode.com/svn/wiki/images/mona_purple.jpg](http://eggbotcode.googlecode.com/svn/wiki/images/mona_purple.jpg)

Buoyed by the result, I was pretty disappointed when the black bulbs arrived. Unfortunately, both were "high quality" -- meaning, the black coating is on the outside, but there is mirroring on the **inside**.  So, while these are really nice black spheres, there's no way to get light out by pecking the outside.  Plus, the matte coating is thick, and the pecking results in a rather crude line.

![http://eggbotcode.googlecode.com/svn/wiki/images/mona_failed.jpg](http://eggbotcode.googlecode.com/svn/wiki/images/mona_failed.jpg)

After a call to ChristmasCentral, I ordered the same (evidently lower quality) brand as the successful gray bulbs (Kohler), in black, and since they arrived have been pecking 24 hrs/day.

Which gets to some of the difficulties.  First off, I'm finding that in order to get clean lines I need to go pretty slow-- like 10-20 st/sec.

![http://eggbotcode.googlecode.com/svn/wiki/images/eggbot_logo.jpg](http://eggbotcode.googlecode.com/svn/wiki/images/eggbot_logo.jpg)

And I've discovered all sorts of gotchas-- like when my wife's Win7 desktop goes into its screensaving mode it also logs her off!  That is why the logo is actually not complete-- the Eggbot extension reported a serial timeout when her screensaver started.  And then of course, there are more upsetting failures.  Like when somewhere between the 7-8 hours into a plot the fricking bulb disintegrates!

![http://eggbotcode.googlecode.com/svn/wiki/images/tess_broken.jpg](http://eggbotcode.googlecode.com/svn/wiki/images/tess_broken.jpg)

What's the deal?  It's just a tiny diamond striking a thin glass membrane a million times!  And I won't get into plotting overnight, only to realize that I didn't set up the bulb carefully enough and the pecking didn't reach the surface in all areas.  Argggh.  But I have gotten lucky a couple times:

![http://eggbotcode.googlecode.com/svn/wiki/images/tess_purple.jpg](http://eggbotcode.googlecode.com/svn/wiki/images/tess_purple.jpg)
![http://eggbotcode.googlecode.com/svn/wiki/images/americas.jpg](http://eggbotcode.googlecode.com/svn/wiki/images/americas.jpg)

I use the aluminum and steel shaft collars as weights-- both to increase the down force, but also to dampen the vibration a bit (tighter lines?).  Not sure yet if either is helpful.  I have also tried spraypainting eggs and CF bulbs black (the outer glass on the spherical CF bulbs is just protecting the inner twisty, nasty-stuff-containing bulb).  The first paint (Rustoleum enamel) is too elastic and doesn't peck through well.  I'm waiting for "Camouflage" black and black lacquer to dry on eggs and bulbs to see it they will work.  Hopefully, will have pics soon.