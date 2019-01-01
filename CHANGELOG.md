# Changelog

* 1 January 2019
  * All: updated flask highlighting: quality goes first, in maps non-quality flasks get de-emphasized
  * All: updated sounds & minimap icons for patch 3.1 items (abyss jewels, stygian vise, elder/shaper items)
* 17 December 2018
  * Maps & Strict: copied changes from Leveling, with minor modifications to not show low level gems
* 14 December 2018
  * Leveling: 5-link items got a sound in addition to the light beam.
* 11 December 2018
  * Leveling: overhauled highlighting (started using map icons & beams) for: currency, maps, div cards, rare gems, essences, uniques, quest items.
* 7 December 2018
  * All: added highlights for Betrayal Veiled mods and Scarabs.
* 3 September 2018
  * All: highlight new resonators + fossils introduced in Delve
  * Leveling: reduce dropped items spam (prevalent in Delve) by hiding white/blue items with less than maximum linked sockets.
* 29 August 2018
  * All: show corrupted rare items
  * Leveling: added highlights for the new 3.4 currency items. Once I've tested they work I'll roll these out to the other filters. Beams, custom sounds and minimap icons will follow at a later time as well. I'd like to try those out for myself in the game before updating the filter with them.
* 17 August 2018
  * All: show Blood Raiment and Sadist Garb (evastion/ES endgame armour). Blood Raiment has best ES. Sadist Garb has best ES/Evasion balance. Carnal Armour has best ES and mana bonus.
* 8 August 2018
  * All: chisel recipe hammers: visually de-emphasise 0% quality hammers (they stood out too much)
  * Leveling: removed custom logic section content (it's only for my character, not for the generic filter)
* 3 August 2018
  * All: play a "valuable orb" sound for Orb of Chance / Jeweller's Orb / Chisel / Silver Coin
  * Maps/strict: added space for custom logic
  * All: changed some sounds to put more emphasis on more important things
* 21 July 2018
  * Leveling: added location for custom logic
  * All: properly highlight Uul-Netol splinters, instead of treating them like Nets (they're both currency and contain the word "net")
  * Leveling: reduced number of magic and useless items shown
* 3 June 2018
  * All: added highlights for Incursion League items, such as Stone of Passage, Flashpowder Keg, the stackable currencies "Vial of X" and the specific affixes that some items can have when dropped by the Omnitect.
* 25 April 2018
  * Maps/Strict: split Divination Cards into two categories: normal and boring. Boring cards are slightly de-emphasised graphically and play their drop sound at a lower volume. Boring: Rain of Chaos, Scholar, Carrion Crow, Thunderous Skies. More will likely join this group as I encounter them.
* 16 April 2018
  * All: added highlighting for tier 10 nets: Thaumaturgical Net (can't believe I missed this one).
  * All: top-tier nets play the "an orb of great power" sound instead of the generic currency sound. This affects Necro, Thaumaturgical and Strong Steel Nets. I hope this helps to discern good net drops from regular currency drops (because for good nets you might want to look around, just like for fuses and such)
* 8 April 2018
  * Maps/Strict: highlight maps-tier nets with custom colors
  * Leveling: highlight all nets in addition to the map-tier net highlighting used in maps
* 29 March 2018
  * Leveling: Tweaked the quality of wapons/armour showing to include magic items, and moved the show/hide threshold for armour to 14% (any 3x of these will give currency) and for weapons highlight 14%+ different from 10%+
* 27 March 2018
  * Leveling: Show weapons + armour with 10% quality or more, except for the very bulky ones (large bows, tower shields, staves). This helps with the 40% quality recipes to get whetstones and armour scraps.
* 19 March 2018
  * Leveling: only show Tower Shields with more armour than lower level ones (there's a few large "gaps" with higher level shields that are worse than the lower level one).
* 28 January 2018
  * Maps: Show rare items that take less than 6 inventory squares, regardless of level. Lower level ones are smaller than higher level ones. This helps to get lower tier orbs from selling rares.
* 22 January 2018
  * All: Shaper and Elder item highlights are much more obvious. Entire background now has a different colour instead of only the border.
* 16 January 2018
  * Maps: engame tier items: only show rares, and white items only when max linked sockets is 3 or 4 (1-hand weapons, non-body armour) or 4+ total sockets when max is 6 (armour, bows, staves, 2-handers)
* 8 January 2018
  * All: changed highlighting of drop level 62+ itemw with max 3 or 4+ socket items from purple edge to white edge. It's less attention grabbing this way.
  * Leveling: 3 and 4+ socket items no longer have a transparent background. This makes sense for maps filters, because there's plenty of items there and you really only want the best, but while leveling you simply want upgrades so don't reduce the visual noise just yet.
  * Maps + strict: only show rare+ quivers, not white/magic.
* 18 December 2017
  * Leveling: be a bit less strict about showing items with lower socket counts.
  * Leveling: hide trash magic weapons/armour after act 2 (only show 3/4 linked equippables)
* 10 December 2017
  * FIX: "ShaperItemItem" was not a thing, it's supposed to be "ShaperItem".
* 9 December 2017
  * Removed duplicate listing of Abyss Jewels. They are nice, but no need to show them twice :-)
* 7 December 2017
  * Moved my 3.0 filters from a single gist to a Github repository, so it's easier to browse the filters.
  * Cleared the individual filters' changelogs and gave them all a short pointer to this repository.
  * Backported tiered gem highlighting from Maps to Leveling filter, but actually show all gems while Leveling.
  * Backported top-end wand highlighting from Strict to Maps and Leveling filters.
  * Removed individual changelogs, and added a last changed date to each instead.
  * Added lines to highlight the [Abyss League items](https://www.pathofexile.com/forum/view-thread/2036673)
