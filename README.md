# Compose-and-Program-Music-in-Python-using-Earsketch
### Create a account(Sora2) in Earsketch
- Explore the API in left menu to add music and effects.
```python3
#		python code
#		script_name:
#
#		author:
#		description:
#

from earsketch import *

init()
setTempo(120)
#Music
#   Making variables for song name
chord = RD_UK_HOUSE__5THCHORD_2
secondaryBeat = HIPHOP_BASSSUB_001

fitMedia(chord, 1, 1, 16)
# Add effect between measures 1 and 16 from -60db to 5db and back down
setEffect(1, VOLUME, GAIN, -60, 1, 5, 12)
setEffect(1, VOLUME, GAIN, 5, 12, -60, 16)
fitMedia(secondaryBeat, 2, 1, 12)
#Add effect
setEffect(2, DELAY, DELAY_TIME, 500)
fitMedia(HOUSE_MAIN_BEAT_003, 3, 1, 8)

fitMedia(COMMON_LOVE_DRUMBEAT_1, 4, 5, 12) #my own
#Add effect
setEffect(3, REVERB, REVERB_TIME, 200)
#Finish
finish()
```
