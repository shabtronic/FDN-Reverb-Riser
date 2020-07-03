# FDN-Reverb-Riser

**Info:**

Simple FDN slow attack reverb with shimmer feedback loop

The current algorithm topology is:

**8 Serial Allpass filters in a feedback loop with Modulation,EQ and PitchShifting - into a 4x4 FDN matrix**

FDN is based on the works from

REDUCING ARTIFICIAL REVERBERATION ALGORITHM REQUIREMENTS
USING TIME-VARIANT FEEDBACK DELAY NETWORKS
By
Jasmin Frenette 

http://pages.infinit.net/jfrenett/thesis.pdf

**Reaper JS Version** 

currently using a small UI/DSP lib: https://github.com/shabtronic/ReaperJSLib
 
**VST2/VST3**
 
uses the marvelous IPlug2 library https://github.com/iPlug2/iPlug2

Currently only the UI code is in place - no DSP at the moment.


![](./Images/FDN-Riser-CurrentVersion.png)


## Presets

**Default**

  Medium hall type reverb.

**Chorus Detune**

  Poor mans chorus - sounds like a out of tune piano!

**Stereo Swell**

  Medium decay reverb - that pans across the stereo field.

**Event Horizon**

  The classic "Big Space" FDN sound - endless floaty space (almost).
 
**Orchestra Swell**

  My favourite preset - play with the feedback to control the harmonics and intensity of the swell.
  Works best with sounds that have low to medium harmonic content (nylon guitar, flute e.t.c.)

**Drum Rev**

  Small reverse rise, that works well with drums and gives a gated reverb effect.


All preset examples are here:
 
 https://soundcloud.com/shabtronica/sets/fdn-reverb-presets

## Installation

**VST2 Version**

copy FDNRiser_x64.dll into your normal vst plugins directory, wherever you have previously installed vst2 plugins.

**VST3 Version**

copy FDNRiser.vst3 into your \Program files\Common Files\VST3 directory (must be this directory apparently).

**Reaper JS Version**

Simply copy the three files:

"FDN Verb Riser"
"FDN Verb Riser.rpl"
"stronic-lib.js-inc"

into your \reaper\effects\ directory.

The reverb will then appear in the JS fx list as "FDN reverb riser" once it's been refreshed (either restarting reaper or scan for new plugins).

you may have to import the .rpl into the fx to get the presets.

## Development thread:

https://www.kvraudio.com/forum/viewtopic.php?f=33&t=547140

## To do ##

Add some time change code - resample time, resample pitch or XFade sled - to smooth out any time changes.
