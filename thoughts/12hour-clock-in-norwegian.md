If you really want to announce round timestamps in 12 hour format; at least it should also append something that indicates wheter it's the day or night, otherwise it adds ambiguity that isn't there in the source.

Unfortunately we do not have a consistent equivalent to AM/PM in English; well "formiddagen" and "ettermiddagen" historically did (though I think it was only used for times during the day),
but because "middag" also is the name of the main meal that to day is normally eaten around 16:00 - 17:00 theres considerable confusion on when these times is,
older people generally think "formiddag" is between "morgen" and 12:00, and "ettermiddag" is after 12:00 to "kveld" (and "morgen" and "kveld" seems to be very roughly twilight +/- a few hours which changes considerably through the year).
Younger people seem to think "formiddag" is between whenever they have lunch (typically sime time betwee 11:00 and 14:00) and whenever they have dinner (typically 15:00-18:00).
So when a younger person say "formiddag" they might very well talk about some time an older person would consider "kveld" in winter because it's long after dark.


I suggest we just avoid using "formiddag" and "ettermiddag" completelly and use "dagen" to refer to the day hours that cannot possibly be considered morning (which historically technically would be ettermiddag)

In theory you could use only two suffixes, "om natten" (in the night) and "om dagen" (in the day), which is what we often do in actual spoken Norwegian when talking informally and in-person (in any more precise or formal setting, we almost exclusively use 24 hour time, usually including leading and trailing zeroes to make it obvius that it is 24 hour format); which works fine for any time between in the  10:00 to 17:00 range and 22:00 to 05:00 range, because "everyone" agrees that those times are clearly day-time and night-time respectively. But outside that it becomes very ambigous and it really depends on whether you're speaking to a morning person or a night owl as most people would consider the time they are definitely asleep as "night"; so to a night owl 06:00 is in the middle of the night, while to a baker it's early in the day; which means you need to know who's speaking to know wether "seks om natta" is 06:00 or 18:00, which doesn't work for a generic robot voice that has to be unambiguous.

I think the best approach is dividing the day into four six-hour chunks like so:

00:00 - 05:59 could be "klokka TIMESTAMP_HERE om natta"
06:00 - 11:59 could be "klokka TIMESTAMP_HERE om morgenen"
12:00 - 17:59 could be "klokka TIMESTAMP_HERE om dagen"
18:00 - 23:59 could be "klokka TIMESTAMP_HERE om kvelden"

This makes most sense to me and is not that far off from most Norwegians's idea of when the terms are. And because it's 4 chunks,
even if you disagree with the exact starting points there's no ambiguity.


---

That said; I personally prefer (and I think most Norwegians under 40 would agree with me), that it just reads all 24-hour times as it's written,
i.e.: 18:15 is "(klokka) atten femten".
