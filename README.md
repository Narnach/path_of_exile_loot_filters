# Narnach's Loot filters for Path of Exile

(Last major patch update: 3.5 / Betrayal League)

These are the [Path of Exile](https://www.pathofexile.com/) loot filters I use in my recordings over at [youtube.com/narnach](https://www.youtube.com/narnach)
It keeps evolving over time, as my needs keep changing and new things get added to the game over time. Make sure to check back [here](https://github.com/Narnach/path_of_exile_loot_filters) every once in a while. My biases are towards my playstyle and my needs. Yours may be different.

This collection of loot filters started a just a simple loot filter that I played with when the feature got introduced in Path of Exile 2.0. Over time it's evolved to a collection of loot filters for different stages of the game:

- [Leveling](https://github.com/Narnach/path_of_exile_loot_filters/raw/master/Narnach-Leveling.filter): A general purpose filter to use while leveling, with a focus on showing the items that are appropriate to your current area level, or about 5 below it.
- [Maps](https://github.com/Narnach/path_of_exile_loot_filters/raw/master/Narnach-Maps.filter): A filter to use when you're running maps. It hides low level items, but still show endgame crafting bases and potentially valuable items to use or trade away.
- [Strict](https://github.com/Narnach/path_of_exile_loot_filters/raw/master/Narnach-Maps-Strict.filter): A filter that is useful once you are established in maps, and just want all the "junk" items to disappear. This is the strict loot filter to keep your screen mostly free of visual noise.

Originally I hosted my filter in a Gist on Github, but as I've added more filter files, that became cluttered and difficult to use. This repository solves that organisational problem!

Each loot filter traditionally had its own changelog listed near the top, but I'll replace that with a single [Changelog](CHANGELOG.md).

## How to use these filters

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
