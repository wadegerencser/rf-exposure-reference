# The Part Nobody Brings Up

I want to say up front that this is not a warning. Nothing in here is going to tell you that your
phone is dangerous or that the access point over the conference room table is doing something to you.
The arithmetic does not support that, and I am not interested in making a claim the numbers do not
back.

What I am interested in is a narrower thing that does not get brought up much. Almost every
reassuring statement about RF exposure is a statement about normal use at normal distances. A ceiling
mounted access point two and a half meters over somebody's head is running at something like a tenth
of one percent of the FCC general population limit, and that is before you give it any credit for the
fact that Wi-Fi is bursty and mostly idle. That is not a close call. It is not worth anybody's
anxiety.

But that is not the only way people end up around this equipment.

## Think about how the work actually gets done

Somebody has to stage the gear. I have been in rooms where twenty or thirty access points are sitting
on folding tables, all powered up, all beaconing, getting adopted and provisioned and firmware
flashed, while a couple of people sit right there working through the list for hours. I have seen
radios on a bench at arm's length being driven to full power on purpose because that is what the test
called for. I have watched people troubleshoot a directional antenna by standing in front of it. Lab
gear gets handled at 30 centimeters, not at 2 meters, and it gets handled all day.

That is a different exposure situation than the one all the reassuring numbers describe. Not because
the equipment changed. Because the distance changed, and the duration changed, and the number of
transmitters changed.

Here is what the math says, using the same free space formula the FCC uses for this class of
evaluation, and using the general population limit of 1.0 mW/cm2 for frequencies above 1500 MHz.

| Situation | Percent of general population limit |
|---|---|
| One AP at 30 dBm EIRP, 2.5 m away, ceiling mounted | 0.13 percent |
| One AP at 30 dBm EIRP, 50 cm away on a bench | 3.2 percent |
| Eight APs at 30 dBm, 50 cm, all transmitting | 25 percent |
| Sixteen APs at 30 dBm, 50 cm, all transmitting | 51 percent |
| One standard power radio at 36 dBm EIRP, 20 cm | 79 percent |
| One standard power radio at 36 dBm EIRP, 10 cm | 317 percent |

Those last two are the ones that get my attention. A 36 dBm EIRP radio reaches the general population
limit at about 18 centimeters. That is not a hypothetical number. That is a hand's width.

## The honest caveats, because they matter

I have to put the qualifiers on this, and they are real ones.

Those bench numbers assume 100 percent duty cycle, which no Wi-Fi radio actually does. Real APs on a
staging table are beaconing and mostly idle, so knock a factor of ten or more off. The eight AP row
at a realistic 10 percent duty cycle is about 2.5 percent of the limit, not 25. Wi-Fi being bursty is
doing a lot of quiet work in your favor.

Those numbers also use the general population limit. Somebody working around transmitters as part of
their job may fall under the occupational limit instead, which is five times higher, on the
assumption that they are trained, informed, and can control their own exposure. That assumption is
the part worth pausing on. It is not a claim that workers are tougher. It is a claim that they know
what they are standing next to. If nobody ever told them, the assumption is not being met.

And the free space formula stops being valid up close. Inside the near field, which for these
frequencies is only a few centimeters, you cannot calculate it this way at all. That is exactly why
devices used against the body get SAR tested in a phantom instead. So the 5 and 10 centimeter numbers
should be read as an indication of scale and not as an assessment.

Even with all of that, the point survives. Distance and duration and transmitter count are the whole
ballgame, and the staging bench is the one place in this industry where all three of them go the
wrong direction at the same time.

## Why I care about this more than most

I did not come into RF through Wi-Fi. I came into it through the Marine Corps, working on the EA-6B
Prowler. The Prowler was a tactical electronic countermeasures aircraft and the entire point of it was
radiating high power RF on purpose, out of external jamming pods driven by ram air turbines, to put
enough energy into a radar environment to blind it. Being on a flight line around that aircraft is not
the same experience as reading a datasheet.

Something that was noticed and talked about across the four Marine Corps Prowler squadrons was that
the kids of the pilots and aircrew were almost all girls. Almost every family. That is an observation
from inside a community and it is not a study. There were probably a boy or two somewhere that I did
not know about, and small groups of people come out lopsided by chance all the time. I am not putting
it forward as proof of anything and it is not meant as a sting at anybody. It just stayed with me.

So I went and looked at what has actually been published on that specific question, expecting to find
nothing. That is not what I found. A cross sectional study of 10,497 men in the Royal Norwegian Navy
reported a dose related increase in infertility and a significant trend toward fewer boys as reported
exposure to high frequency aerials went up. A meta analysis published later pooled the wider
occupational literature and found no association with sex ratio at all. Both of those are published.
Neither one settles it. The citations are in the reference, along with the animal work and where its
dose levels actually sit.

What does not exist, as far as I can tell from searching the indexed literature, is any study of
aircrew on tactical electronic warfare platforms. Not a reassuring one and not an alarming one. Just
nothing. That is worth saying plainly, because an absence of study is not the same thing as a finding
of safety, and it gets treated as one all the time.

## What I actually want out of this

Not fear. There is plenty of that already and most of it is aimed at the wrong targets, at routers and
at towers and at phones, where the numbers are genuinely not close.

What I want is for the people who work close to this equipment for long stretches to know the numbers
for their own situation, because those numbers are public, they are not hard, and almost nobody has
ever been shown them. If you stage APs, if you work a test bench, if you are the one standing in front
of the directional antenna while somebody else reads the meter, the arithmetic that applies to you is
not the arithmetic in the marketing material.

Three things that are free and actually work:

1. Distance. Doubling it cuts power density by a factor of four. Moving a bench radio from 20
   centimeters to 60 does more than any other single thing available to you.
2. Do not sit in the boresight. Antenna gain is redistributed power, not free power. A 15 dBi
   directional antenna is putting roughly 32 times the density on axis compared to isotropic, and much
   less everywhere else. Where it points is part of the answer.
3. Power the bench down when you are not testing at full power. Most staging work does not need
   maximum EIRP. If it does, use the distance.

That is the whole message. It does not apply to most environments and I want to be clear about that.
It applies to the ones where somebody sits close to a lot of transmitting equipment for a long time,
which happens to be how a fair amount of this industry actually gets built.

The full reference, with the physics, the regulatory framework, the device comparisons, a live
calculator you can put your own numbers into, and the studies with their citations and their
limitations, is here:

https://wadegerencser.github.io/rf-exposure-reference/

Run your own scenario in the calculator rather than taking my word for any of it. That is sort of the
point.
