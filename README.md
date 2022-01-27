# This filter is retired

I've decided to retire this loot filter. I'm no longer as active in PoE as I was in the past when I still made YouTube content, and I find it increasingly less motivating to keep this filter up-to-date.

I recommend you have a look at [Filterblade](https://www.filterblade.xyz/) which is an excellent way to customize Neversink's filters to your liking.

# Narnach's Loot filters for Path of Exile

(Last major patch update: 3.15 / Expedition League)

These are the [Path of Exile](https://www.pathofexile.com/) loot filters I use in my recordings over at [youtube.com/narnach](https://www.youtube.com/narnach)
It keeps evolving over time, as my needs keep changing and new things get added to the game over time. Make sure to check back [here](https://github.com/Narnach/path_of_exile_loot_filters) every once in a while. My biases are towards my playstyle and my needs. Yours may be different.

This collection of loot filters started a just a simple loot filter that I played with when the feature got introduced in Path of Exile 2.0. Over time it's evolved to a collection of loot filters for different stages of the game, then it got unified into one SSF loot filter.

## SSF Loot Filter

[SSF](https://github.com/Narnach/path_of_exile_loot_filters/raw/master/Narnach-SSF.filter): My new (as of PoE 3.13) unified loot filter. It scales from level 1 to 100, slowly getting stricter as you need it. Here's what it does:

It separates the filter into multiple stages. This is a rough breakdown:

- **The highlight stage**. Here it highlights things with special properties, giving it a specific text color, border, background, minimap icon or light beam. Right now it handles: corrupted items, RGB socketgroups and a default background color for currency. There's also a default fallback for unfiltered items which will give them a red beam and a red kite minimap icon. This is for debugging and future-proofing. A new item class will catch your attention this way.
- **Maps**. These have their own section because they have their own rules. Maps' background color matches their tier: white/yellow/red. Their borders, beam & minimap icon are red when it's a higher tier than your current map. Non-higher level maps of the same tier (white/yellow/red) have a yellow outline. One tier lower (white in yellow, yellow in red) is outlined in blue and two tiers lower (white maps dropping in red maps) are white.
- **Baseline items to always show**. Some items are always useful for all builds. Currency, maps, 6-links, etc. This stage has five levels of importance. Each stage has a primary color used in highlights and the minimap to help you recognize it, following the normal item color progression: orange/gold are top-tier items, yellow are high-tier, blue is mid-tier, white is low-tier and gray is trash-tier.
  - Top: you expect to see very few of these, and you would backtrack your entire map to pick them up. Examples: Exalted Orb, Mirror of Kalandra, 6-linked items, awakened or alternate quality gems.
  - High: you expect to see these every couple of maps, and would backtrack multiple screens to pick them up. Examples: most Unique items, Regal Orb, Vaal Orb, Orb of Fusing, high-tier Essences, high-tier Oils, not-common Divination Cards. Most league-specific items are here, though they have purple (current) and pink (old) as their highlight colors. Those are becoming more accessible via Heist and other cross-league drop mechanics, so at some point might get folded into the regular blue/yellow tiers because they are no longer special.
  - Mid: you expect to see multiple of these each map, so you might not backtrack more than a screen. Examples: Chromatic Orb, Alchemy Orb (in maps), common Divination Cards, most currency Shards, low-tier Essences, gems/flasks with 10+ quality, rare jewels, low-tier Oils, 6-socketed items, maps-only base items. Drop-only gems.
  - Low: low quality gems & flasks, low-tier currency and shards.
  - Trash: scrolls (from act 6)
- **Leveling curve items**. This is where most of your gear goes: weapons, armour, flasks without quality.
  - **Gems without quality**. Show all gems (without quality) until you can buy them. Library-buyable gems disappear in Act 4. The rest you can buy disappears in Act 6. The exception is gems with experience (from chests).
  - **Flasks without quality**.
    - Utility flasks have Cyan beams until Act 6, then show with a highlight and disappear in yellow maps.
    - Life/mana flasks have their own progression, showing the current two tiers of flasks. The level 42 flasks are really good, so those stay visible until they get replaced at level 60. Non-quality flasks disappear in maps.
  - **Corrupted items**. You can't craft them, so normal & magic ones are hidden.
  - **Jewelry**. I tend to craft white ones into rares early on, then mostly give this up in the endgame in favor of examining each rare one. Vaal Orbing jewelry means the base item is less important if the stats are good, so treat them all the same when rare. Rules: show all jewelry in act 1 and 2, hide magic jewelry from act 3, show normal jewelry as faded from act 6, fading them even stronger in maps.
  - **Gear**. We have different phases here as well.
    - The base rule is to hide normal & magic items whose minimum DropLevel are 10+ levels too old. (i.e. not worth using as crafting bases)
    - Next, show all rares whose DropLevels are within the last 15 levels. (i.e. worth evaluating for use)
    - Afterwards, hide items for which sockets are not good enough. Having 4+ linked sockets is good, as is 3 linked sockets on shields and 1-handed weapons. Until act 3 we can't even get 4 sockets, so highlight 3-links, do a more subtle highlight for 3-sockets.
    - Lastly: the leveling curve. In acts 1-5 show all outdated rares with a faded background. They might still work for vendoring or if you are unlucky with drops. Act 1 shows all 3-links. Act 2 hides items with 1 or 2 sockets. Act 3+ items which can have 4+ sockets are hidden with less than 4 sockets.

The Gear section has a TODO to re-generate it using a script which uses item data from PoE's website, so we can determine T1, T2 and T3 for each level range for each item type, accounting for DPS, attack speed, implicits, etc. This would help account for weirdness such as a lot of tower shields getting much worse armour during certain parts of the leveling curve, so the T1 stays the same for 20+ levels. Maraketh items with their unique implicits also fall in their own curve which is currently not yet accounted for.

### Old filters

These filters have last been updated for 3.13 Ritual League and probably won't get updated anymore.

- [Leveling](https://github.com/Narnach/path_of_exile_loot_filters/raw/master/Narnach-Leveling.filter): A general purpose filter to use while leveling, with a focus on showing the items that are appropriate to your current area level, or about 5 below it. As you progress through the game, it will hide more and more useless items and only show you (potentially) helpful items.
- [Maps](https://github.com/Narnach/path_of_exile_loot_filters/raw/master/Narnach-Maps.filter): A filter to use when you're running maps. It hides low level items, as well as most useless items. It stills show endgame crafting bases and potentially valuable items to use or trade away.
- [Strict](https://github.com/Narnach/path_of_exile_loot_filters/raw/master/Narnach-Maps-Strict.filter): A filter that is useful once you are established in maps, and just want all the "junk" items to disappear. This is the strict loot filter to keep your screen mostly free of visual noise. Mostly shows currency and guaranteed helpful items.

Originally I hosted my filter in a Gist on Github, but as I've added more filter files, that became cluttered and difficult to use. This repository solves that organisational problem!

Each loot filter traditionally had its own changelog listed near the top, but I'll replace that with a single [Changelog](CHANGELOG.md).

## How to use these filters

There's always a copy of the latest filters on [my profile](https://www.pathofexile.com/account/view-profile/narnach/item-filters) on the Path of Exile website.

If you only want a single filter, then simply copy the Raw text of the filter (follow the links above) and store it in a file in this directory:

`C:\Users\<USERNAME>\Documents\My Games\Path of Exile\`

The file MUST have the ".filter" extension, for example `Narnach-Strict.filter` would be a good loot filter file name.

After you have stored the file, inside of Path of Exile, go to Options -> UI -> <Scroll down to the bottom> -> Select the filter from the pulldown -> Click "Reload".

If you want to use all the filters, and easily keep them up to date, you could consider using the Github Desktop client to clone this repository into the directory mentioned above. That's what I do myself so I can easily share the changes I make.

## About loot filters, or how to customise this

A very handy page to bookmark is the [Wiki Guide](https://pathofexile.gamepedia.com/Item_filter_guide) and [Wiki Page](https://pathofexile.gamepedia.com/Item_filter) for ItemFilters. Other than that, just before each new league, a news post like [this](https://www.pathofexile.com/forum/view-thread/2036673) will be posted by the devs that lets us know how the new expansion is going to impact loot filters. It is very useful to update your loot filter at least once before you play the new league, so you won't miss out on the new things.

## TODO

A loot filter is rarely finished. Here is a list of things I still intend to change.

* See if I can simplify some rules and re-think the layout of the filter files. With three files, it'd be nice to have some sections that are always the same, and clearly marked sections that are different.
* It is my intention to eventually merge the Leveling filter into the Maps filters, and only have a Strict and a non-Strict version of the same filter. This ties in with the previous point of re-thinking my filter layout. I might have to resort to using different raw files to store sections and then using a script to merge them together. We'll see what I'll end up doing.

## Attribution

By now, these filters are my work entirely, but back in the 2.0 beta I got started by tweaking Quill18's Simple LootFilter, which you can find [here](https://gist.github.com/quill18/d811f616d577bed035b4).

## About me

I'm Wes "Narnach" Oldenbeuving, freelance [software developer](http://narnach.com) by day and [Youtuber](https://www.youtube.com/narnach) by night. I tend to start at least one character every Path of Exile league. I don't enjoy cookie cutter builds, and record most of my PoE gameplay as Let's Play series. Solo self-found, often on hardcore, is my thing.

* YouTube: https://www.youtube.com/narnach
* Twitch: http://www.twitch.tv/narnach
* Twitter: https://www.twitter.com/narnach
* Old Gist: https://gist.github.com/Narnach/79e57e9846851e69eb01
