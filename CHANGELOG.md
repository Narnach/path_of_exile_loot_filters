# Changelog

* 25 July 2021
  * SSF: all Expedition "reset" currencies are marked as rare currency
  * SSF: recolorize Expedition currency
* 24 July 2021
  * SSF: added Warstaves everywhere Staves are referenced (they are not included otherwise)
* 23 July 2021
  * SSF: beta 3.15 compatibility update. Add all new items as league-specific (purple highlight), change Ultimatum to "old league" highlight (pink) and add new Flask-related currencies at Chaos Orb equivalent tier (high rarity). No changes seem required to account for new gems and flasks.
  * SSF: renamed Blessed Boots to Fugitive Boots, correcting the one typo in the initial release
* 17 April 2021
  * SSF: stop highlighting jewelry with a different background color, it's too distracting
* 16 April 2021
  * SSF: start de-emphasizing jewelry at level 30 instead of 45
  * SSF: items with 1-9 quality are no longer auto shown; 10-19 gets the highlight, but still follows display rules
  * SSF: added support for 3.14 / Ultimatum base items
* 11 March 2021
  * SSF: show more items as faded on area level 1-4 to help new characters
  * SSF: show relevant items with quality (highlight tiers 20+, 10+, 1+)
* 25 February 2021
  * SSF: Introduced a new loot filter as "stable": the SSF filter. This one is unified to work for both leveling and maps. It gets stricter after certain thresholds: level 4, act 1, act 3, act 5, white/yellow/red maps. Highlighting is based on the needs of a SSF player, so early on you want 3 sockets on any item, then 3 linked sockets, then 4 sockets, then 4 linked (end of act 4). Once you hit maps, care about decent crafting bases (T1 bases) but rares for T1-3 bases are all still fine to ID and enhance via crafting. Currency follows a similar curve: you want everything in act 1, then slowly you get lazier about low-tier currency such as scrolls, then transmutes and even alterations.
* 16 January 2021
  * All: applied Ritual / Echoes of the Atlas changes.
* 15 January 2021
  * Leveling: applied QoL changes from Heist league: contracts have different color, all Atlas influence items have a highlight, large Chromatic items are hidden after level 45, non-quality Gems stop showing once you can buy them (level 30, 45)
* 19 September 2020
  * All: Compatibility update with 3.12, Hesit League. New alternate quality gems, replica relics, experimental base types and Heist-specific currency and league items.
  * Leveling: apply some old Harvest colors
* 20 June 2020
  * All: Compatibility update with 3.11, Harvest League. New currency, goddess offerings, harvest seeds.
* 13 March 2020
  * All: Compatibility update with 3.10, Delirium League. Cluster Jewels, Simulacrum / splinters, Delerium Orb
* 14 December 2019
  * Maps: highlight map-specific base items with a blue beam
  * All: Compatibility update with 3.9 (renamed Warstaff to Warstaves, Sextant lost the Cartographer's bit)
  * All: added 3.9 items: Metamorph samples, Catalysts,  "Awakener's Orb", Ivory Watchstone, Awakened gems. Other new items were already in suitable categories based on my initial estimate.
* 18 September 2019
  * All: highlight Vermillion Ring, Cerulean Ring and Convoking Wand, new item base types
* 8 September 2019
  * Leveling: Flasks only show in wider level ranges in acts 1-3; afterwards it became too noisy (partial revert of earlier changes)
* 7 September 2019
  * All: highlight Blighted maps with a nice sickly green color.
  * All: highlight Oils with custom color.
  * Leveling: show flasks a little longer (show current + previous tier instead of only current tier)
  * All: Highlight Warstaff and Staves where previously it was only Staves
* 13 June 2019
  * Leveling: don't hide non-4-linked items until act 5 (instead of act 4). This gives you a little more time to pickup those 4 socketed but not linked items while leveling.
* 7 June 2019
  * All: added patch 3.7 / Legion loot highlights (Incubators/Blessings/Splinters)
* 23 May 2019
  * All: highlight Perandus Coins as medium tier currency.
  * All: better highlight Breach Splinters on par with medium tier currency.
* 9 March 2019
  * All: added highlights for Synthesis league items
* 1 January 2019
  * All: updated chaos/regal recipe jewelry highlight: de-emphasize these drops because they are not that important
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
