# Relics of Hyrule - GAT Edition
- [Relics of Hyrule - GAT Edition](#relics-of-hyrule---gat-edition)
- [Preamble](#preamble)
- [Installation](#installation)
  - [Pre-Installation](#pre-installation)
    - [Installing Microsoft Visual C++ Redistributable Package](#installing-microsoft-visual-c-redistributable-package)
    - [Skyrim Anniversary Edition and Wabbajack](#skyrim_anniversary_edition_and_wabbajack)
    - [Steam Config](#steam-config)
      - [Disable the Steam Overlay](#disable-the-steam-overlay)
      - [Change Steams Update Behavior](#change-steams-update-behavior)
      - [Set the Game language to English](#set-the-game-language-to-english)
    - [Clean Skyrim](#clean-skyrim)
    - [Start Skyrim](#start-skyrim)
  - [Using Wabbajack](#using-wabbajack)
    - [Preparations](#preparations)
    - [Downloading and Installing](#downloading-and-installing)
    - [Problems with Wabbajack](#problems-with-wabbajack)
  - [Post-Installation](#post-installation)
- [Updating](#updating)
- [Noteworthy Mods](#noteworthy-mods)
  - [Combat - Melee](#combat---melee)
  - [Combat - Magic](#combat---magic)
  - [Skills, Perks and More](#skills-perks-and-more)
  - [Quest and Encounter Mods](#quest-and-encounter-mods)
  - [Expanded Cities Towns and Villages](#expanded-cities-towns-and-villages)
  - [NPC Retextures](#npc-retextures)
  - [Followers](#followers)
  - [Audio and Weather](#audio-and-weather)
  - [New Equippables](#new-equippables)
- [In-Game MCM Options](#in-game-mcm-options)
  - [CGO](#cgo)
  - [Immersive HUD](immersive-hud)
  - [Sky UI](#sky-ui)
  - [Skyrim Unbound Reborn](#skyrim-unbound-reborn)
- [Character Creation](#character-creation)
- [Getting Started in Game](#getting-started-in-game)
- [FAQ](#faq)
- [Tweaking Performance](#tweaking-performance)
  - [Tweaking the ENB](#tweaking-the-enb)
  - [Tweaking the Game Settings](#tweaking-the-game-settings)
- [Removing the Modlist](#removing-the-modlist)
- [Credits and Thanks](#credits-and-thanks)
- [Contact](#contact)
- [Contributing](#contributing)
- [Changelog](#changelog)

# Preamble
![rge](extra/rge.png)

The goal of this modlist is to be something fun and different rather than
your 100th enai-survival-rim playthrough.
Please check your immershun at the door and embrace that c0da makes it canon!

This modlist primarily revolves around [Relics of Hyrule](https://www.nexusmods.com/skyrimspecialedition/mods/12244) and [Grand Admiral Thrawn](https://www.nexusmods.com/skyrimspecialedition/mods/24) with new monsters coming from a heavily modified version of [Rogue-Like Encounters](https://www.nexusmods.com/skyrimspecialedition/mods/23872).

Combat is mostly handled by [AGO](https://www.nexusmods.com/skyrimspecialedition/mods/24296), [CGO](https://www.nexusmods.com/skyrimspecialedition/mods/33767) and [SkyRe](https://www.nexusmods.com/skyrimspecialedition/mods/17915). Enemy AI and new monsters are provided by [RLE](https://www.nexusmods.com/skyrimspecialedition/mods/23872) while both player and npc dodging come from The Ultimate Dodge Mod.

This modlist does not require downgrading Skyrim from the latest version. 

# Installation

## Pre-Installation

These steps are only needed if you install this Modlist for the first time. If you update the Modlist, jump straight to [Updating](#updating).

### Installing Microsoft Visual C++ Redistributable Package

I doubt you need to do this since you likely already have this installed. The package is required for MO2 and you can download it from [Microsoft](https://support.microsoft.com/en-us/help/2977003/the-latest-supported-visual-c-downloads). Download the x64 version under "Visual Studio 2015, 2017 and 2019". [Direct link](https://aka.ms/vs/16/release/vc_redist.x64.exe) if you can't find it.


To prevent your game updating, change Skyrim SE's update settings in Steam to only update when launched. Never launch Skyrim SE via Steam, only via your mod manager or skse64_loader.

Please do not ask when AE will be supported.

### Steam Config

#### Disable the Steam Overlay

The Steam Overlay can cause issues with ENB and is recommended to be turned off.

Open the Properties window (right click the game in your Library->Properties), navigate to the _General_ tab and un-tick the _Enable the Steam Overlay while in-game_ checkbox.

#### Change Steams Update Behavior

SSE is still being updated by Bethesda (they only add Creation Club content). Whenever the game updates, the entire modding community goes silent for the next one or two weeks because some mods need to be updated to the latest game runtime version.

To ensure that Steam does not automatically updates the game for you, head over to the Properties window, navigate to the _Updates_ tab and change _Automatic updates_ to _Only update this game when I launch it_. You should also disable the Steam Cloud while you're at it.

#### Set the Game language to English

Just do it. This entire Modlist is in English and 99% of all mods you will find are also in English. I highly recommend playing the game in English and **I will not give support to people with a non-English game**.

Open the Steam Properties window, navigate to the _Language_ tab and select _English_ from the dropdown menu.

### Clean Skyrim

I highly recommend uninstalling the game through Steam, deleting the game folder and reinstalling it. You should also clean up the `Skyrim Special Edition` folder in `Documents/My Games/`.

### Start Skyrim

After you have done everything above and got a clean SSE installation ready, start the Launcher and open the _Options_ menu.

1. Click on _High_
1. Set the _Aspect Ratio_ and _Resolution_ to your monitor's native values
1. Set _Antialiasing_ to _Off_
1. Check _Windowed Mode_ and _Borderless_

Start the game and exit once you're in the main menu.

## Using Wabbajack

### Preparations

Let's get to the actual installation. Grab the latest release of RGE from the Browse Modlists page in the Wabbajack app.

Download the release to a _working folder_. This folder **must not** be in a _common folders_ like your Desktop, Downloads or Program Files folder. It's best to create a Wabbajack folder (the _working folder_) near the root level of your drive like `C:/Wabbajack`.

Grab the latest release of Wabbajack from [here](https://github.com/wabbajack-tools/wabbajack/releases) and place the `Wabbajack.exe` file in the _working folder_.

### Downloading and Installing

The download and installation process can take a very long time depending on your system specs. Wabbajack will calculate the amount of threads it will use at the start of the installation. To have the highest amount of threads and thus the fastest speed, it is advised to have the working folder on an SSD, as should the list install location.

1. Open Wabbajack
1. Click Browse Modlists and find RGE and press the download button.
1. Set Installation Location to where you wish to install the list, which should not be your Skyrim folder or a folder that already has other things in it. This should preferably be a blank folder on the root of your drive, such as F:\RGE if installing it to your F drive. 
1. Set Download Location to where you want mod archives to be, by default it would be a folder named "Downloads" in the list's installation folder. 
1. Click the Go/Begin button
1. Wait for Wabbajack to finish

### Problems with Wabbajack

There are a lot of different scenarios where Wabbajack will produce an error. I recommend re-running Wabbajack before posting anything. Wabbajack will continue where it left off so you loose no progress.

**Could not download x**:

Should this happen it is most likely files from ModDB when trying to install RGE and the exact names of them can be found in your log file or the window in the lower right corner of Wabbajack. 

Should you get a message about being unable to download Skyrim Realistic Overhaul please go to to the following link and download the parts mentioned when you tried to install.
https://www.moddb.com/mods/skyrim-realistic-overhaul/downloads

Other files it can happen on are any that are particulary large, such as Voices EN  - Part 2 or part 1 from the Unofficial High Definition Audio Project, Kart_CSSET_Overwrite from Cleaned Skyrim SE Textures (the pre 1.6 version), both of these are linked below. 

In order to determine the correct page for the file failing to download look at the Wabbajack log file and find the file name. As an example, for the voices file it would be "Downloading Voices EN - Part 1-18115-0-1.7z." The 1 is from part 1 and can be ignored while the 18115 is the mod ID on the Nexus, hence it being in the Nexus link to the page given below. You can use the ID to locate the mod page by replacing the number with the relevant mod ID and finding the correct file in the downloads section. Should you require more help you can find it on the Animoculary Discord server, https://discord.gg/DffHKcszfg. 

https://www.nexusmods.com/skyrimspecialedition/mods/18115 - Unofficial High Definition Audio Project
https://www.nexusmods.com/skyrimspecialedition/mods/38775 - Cleaned Skyrim SE Textures

**x is not a whitelisted download**:

This can happen when I update the modlist. Check if a new update is available and wait if there is none.

**Wabbajack could not find my game folder**:

Wabbajack will not work with a pirated version of the game. If you own the game on Steam, go back to the [Pre-Installation](#pre-installation) step.

## Post-Installation

With the introduction of Stock Game, installing an ENB and Reshade preset yourself is no longer needed and instead the Nyclix preset is preinstalled in the stock game folder. If you wish to change ENB preset or Reshade preset, put the appropriate files in the Stock Game folder. In order to avoid a visual bug that sometimes occurs when loading into the game from the main menu the Reshade preset is turned off by default and can be activated by pressing the Insert key once ingame. 

### Starting the game

To start the game after installing the list go to the folder you have installed the list to and launch ModOrganizer.exe. Select "The Game (AKA SKSE)" from the drop down menu next to the run button and click the run button. If it asks to change your registry so it matches MO2's managed game path, press yes. This is part of the Stock Game folder that lets the list exist indepently of your normal Skyrim installation.

# Updating

If this Modlist receives an update please check the Changelog before doing anything. Always backup your saves or start a new game after updating.

**Wabbajack will delete all files that are not part of the Modlist when updating!**

This means that any additional mods you have installed on top of the Modlist will be deleted. Your downloads folder will not be touched!

Updating is like installing. You only have to make sure that you select the same path and tick the _overwrite existing Modlist_ button.

# Noteworthy Mods

## Combat - Melee

[Combat Gameplay Overhaul](https://www.nexusmods.com/skyrimspecialedition/mods/33767) provides several features and fixes to combat and movement. It has procedural leaning, grip changing, mid-air combat, striking with staffs, dual-wielding two-handed weapons, 1st and 3rd person animations and more.

We use The Ultimate Dodge Mod for all of our fancy dodging needs as the first person dodge of CGO is nausea inducing.

[Skyrim Redone](https://www.nexusmods.com/skyrimspecialedition/mods/17915) covers the rest of the combat mechanics and enemy scaling. I would definitely recommend reading at a minimum Chapter 6 of the SkyRe Guide to see how the combat mechanics affect you.

A heavily modified version of [Rogue-like Encounters](https://www.nexusmods.com/skyrimspecialedition/mods/23872) handles NPC AI, some new combat mechanics and a curated set of new monsters.


## Combat - Magic

Rather than using the usual [Apocalypse](https://www.nexusmods.com/skyrimspecialedition/mods/1090) and calling it a day I have instead opted to include [Forgotten Magic Redone](https://www.nexusmods.com/skyrimspecialedition/mods/12711) and [Spell Siphon](https://www.nexusmods.com/skyrimspecialedition/mods/26627)

SkyRe completely overhauls how vanilla magic works while also adding a plethora of new spells. I suggest reading the SkyRe Guide for more information.

Relics of Hyrule and Grand Admiral Thrawn both include additional unique spells and powers.

## Skills, Perks and More

[Wintersun](https://www.nexusmods.com/skyrimspecialedition/mods/22506) adds religion and worship.

Perk overhauls. For this setup I used [Skyrim Redone](https://www.nexusmods.com/skyrimspecialedition/mods/17915). This perk mod is a comprehensive overhaul for Skyrim. We are using a customized version of the perks (helmless), combat and enemy scaling modules. The SkyRe Guide should be consulted if you want more information. All 'mechanics' and 'content' stuff is still up to date.

If you are are into Spellblade, Arcane Archery, or just magery in general then [Spell Siphon](https://www.nexusmods.com/skyrimspecialedition/mods/26627) is probably the best thing you've never experienced before. Be sure to watch the tutorial video... it's worth it.

Werewolves are overhauled by [Growl](https://www.nexusmods.com/skyrimspecialedition/mods/31245) while [Curse of the Vampire](https://www.nexusmods.com/skyrimspecialedition/mods/10086) takes care of our bloody friends of the night.

[Aetherious](https://www.nexusmods.com/skyrimspecialedition/mods/26686) is a streamlined race overhaul designed to make races more meaningful without making them more restrictive.

[Shout](https://www.nexusmods.com/skyrimspecialedition/mods/12149) improves upon all shouts in Skyrim in a fair and balanced way by cutting down the cooldown timer effects, thus allowing the player to use a host of shouts in innovative, devastating combinations.

[Mundus](https://www.nexusmods.com/skyrimspecialedition/mods/33411) is a streamlined Standing Stone overhaul designed to ensure that every stone fills a niche and offers competitive bonuses to different playstyles.

## Quest and Encounter Mods

RGE comes with a wide variety of new quest and encounters. A few are listed below.

[Darkend](https://www.nexusmods.com/skyrimspecialedition/mods/10423) allows you to travel to the new island of Pharos, explore detailed environments, fight new enemies and discover an Ancient set of weapons of incredible power. There is no quest or hand holding and is heavily inspired by the Soulsborne games.

[Hammet's Dungeons](https://www.nexusmods.com/skyrimspecialedition/mods/12186) and [Land of Vominheim](https://www.nexusmods.com/skyrimspecialedition/mods/31472) add another 60ish high quality dungeons and a landmass the size of solstheim to explore.

[Missives](https://www.nexusmods.com/skyrimspecialedition/mods/17576?tab=files) adds a large number of localized radiant quests found at Missive Boards of varying difficulty and with varying rewards. Missives has been extended to Solstheim.

[Skyrim Sewers](https://www.nexusmods.com/skyrimspecialedition/mods/9320) adds an accessible sewer system to the towns of Solitude, Whiterun, Windhelm and Markarth and also small sewage tunnels to Fort Sungard and Greenwall. Don't let the name fool you as this is by far some of the best made dungeon content available for Skyrim.

[Vigilant](https://www.nexusmods.com/skyrimspecialedition/mods/11849), [Glenmoril](https://www.nexusmods.com/skyrimspecialedition/mods/32998) and [Unslaad](https://www.nexusmods.com/skyrimspecialedition/mods/11789) are an interconnected set of super mods that add a dark and awesome storyline with a ton of Soulsborne inspired content. Glenmoril is still in development but it's worth adding for the current content. Vigilant and Glenmoril creatures and items have been integrated into the rest of the game.

## Expanded Cities Towns and Villages

RGE comes with a massive merge of housing cities towns and villages that overhaul all of the population centers. The list is literally too long to go into in the readme so feel free to check the mod list. There are at least four new player houses per hold ranging from small shacks to massive build your own settlements. The keys for these houses are all purchaseable, found at the end of quests or on enemy corpses. In addition to all of the housing every village town and city has been completely overhauled via a variety of mods.

## NPC Retextures

I love the work of [Pandorable](https://www.nexusmods.com/skyrimspecialedition/users/41216925) and used [Pandorable's NPCs](https://www.nexusmods.com/skyrimspecialedition/mods/19012), [Pandorable's NPCs - Dragonborn](https://www.nexusmods.com/skyrimspecialedition/mods/30680), and [Pandorable's NPCs - Dawnguard](https://www.nexusmods.com/skyrimspecialedition/mods/24135) as my goto NPC retextures.

The Bijin lineup with [Bijin Wives](https://www.nexusmods.com/skyrimspecialedition/mods/11247), [Bijin NPCs](https://www.nexusmods.com/skyrimspecialedition/mods/11287) and [Bijin Warmaidens](https://www.nexusmods.com/skyrimspecialedition/mods/1825) fills the gaps that Pandorable's mods leave.

[The Men of Winter](https://www.nexusmods.com/skyrimspecialedition/mods/10902) retextures some Men in Skyrim. I handpicked NPCs from [Kalilies NPCs](https://www.nexusmods.com/skyrimspecialedition/mods/30247). The rest is covered by [Diversity](https://www.nexusmods.com/skyrimspecialedition/mods/5291). [Ethereal Elven Overhaul](https://www.nexusmods.com/skyrim/mods/24273) is the base for all elves.

The priority looks like this (similar to MO2, the ones at the bottom overwrites the ones at the top):

1. Ethereal Elven Overhaul
2. Diversity
3. Kalilies NPCs
4. The Men of Winter
5. Metalsabers Beautiful Orcs of Skyrim
6. Pandorable's NPCs
7. Pandorable's NPCs - Dragonborn
8. Pandorable's NPCs - Dawnguard
9. Bijin NPCs
10. Bijin Warmaidens
11. Bijin Wives
12. Males of Skyrim
13. Simple Children

## Followers

[Daanik the Returned](https://www.nexusmods.com/skyrimspecialedition/mods/21728/) is a powerful lich boss that you can summon to fight for you assuming that you can defeat him in combat.

[Inigo](https://www.nexusmods.com/skyrimspecialedition/mods/1461) is a fully voiced khajiit adventuring companion with over 7000 lines of unique dialogue - much of it about you. He'll level alongside you and avoid most traps. If you're sneaking he won't chatter and he'll whisper if you talk to him. He can run out of arrows. He's highly skilled in archery, one-handed, and sneak. Do not import Inigo into Amazing Follower Tweaks. 

[Lucien](https://www.nexusmods.com/skyrimspecialedition/mods/20035) is a fully voiced Imperial follower with around 3000 lines of immersive, lore-friendly dialogue. Though he arrives in Skyrim as a cowardly scholar, he'll gradually gain strength and confidence by your side until he grows into a hero in his own right.

[The Pale Lord](https://www.nexusmods.com/skyrimspecialedition/mods/21003) is a uniquely designed vampire follower with both a custom appearance featuring claws and a black textured outfit as well as scripted powers which include the ability to transform into a swarm of bats as well as being able to assume a monstrous War-form.

In addition to the above custom followers all of the vanilla followers have been overhauled by [Special Edition Followers](https://www.nexusmods.com/skyrimspecialedition/mods/7622) to fill unique roles as combat companions.

## Audio and Weather

[Audio Overhaul Skyrim](https://www.nexusmods.com/skyrimspecialedition/mods/12466) and [Immersive Sounds Compendium](https://www.nexusmods.com/skyrimspecialedition/mods/523) offer an amazing base for skyrim's ambiance and foley.

[Soulmancer Music Merge](https://www.nexusmods.com/skyrimspecialedition/mods/22551) thoughtfully merges soundtracks of Celtic Music, Extra Music, Musical Lore, Hun Lovaas, Still, Melodies of Civilization, Vindsvept, Northern & Southern Diaries, Fanmade Nordic Music, Dreams and Nightmares, Elder Songs, Dawn of Hope, and JDR. Additional tracks from Enderal, Two Step's From Hell, Icewind Dale and Baldur's Gate series!

The full Enigma series minus Disciple of Molag Bal from [Satafinix](https://www.nexusmods.com/skyrimspecialedition/users/21706239?tab=user+files) is used to overhaul dragonic and daedric voices. While other odds and ends update draugr voices, skeleton sounds and the like.

[Picturesque](https://www.nexusmods.com/skyrimspecialedition/mods/32364) is a graphical overhaul consisting of a brand new weathers mod along with an ENB preset as companion with a heavy focus on consistency and as few flaws as possible such as matching grass to distant terrain, no horizon seams, decently looking tree LOD. Night-eye, fade to black and other imagespace modifiers are also supported

## New Equippables

[Skyrim Weapon Expansion](https://www.nexusmods.com/skyrimspecialedition/mods/32500) integrates over 100 high quality and balanced weapon variants into the vanilla game through crafting and leveled lists.

[Cloaks of Skyrim](https://www.nexusmods.com/skyrimspecialedition/mods/6369), [Divine Cloaks](https://www.nexusmods.com/skyrimspecialedition/mods/9304), [Daedric Cloaks](https://www.nexusmods.com/skyrimspecialedition/mods/9530) and [Artesian Cloaks of Skyrim](https://www.nexusmods.com/skyrimspecialedition/mods/17416) provide pretty physics enabled capes and integrates them into the world.

[Warmonger Armory](https://www.nexusmods.com/skyrimspecialedition/mods/17809) aims to add immersion to your Skyrim experience adding new lore friendly Armors, Weapons and Clothes for both Vanilla Game and DLCs. All the added content is inspired from the classic Elder Scrolls Archetypes and is made with compatibility in mind.

[Common Clothes and Armors](https://www.nexusmods.com/skyrimspecialedition/mods/21305) is a combined and continued version of Common Clothes and Brigandage. It features 51 new armors and 80 new clothes, created by Franklin Zunge. The clothes are worn by the common people of Skyrim: Farmers, merchants, miners, patrons, workers and some of the wealthier citizens. They can also be bought at Radiant Raiment. The armors are worn by bandits. Since all new armors cover the whole body, half-naked bandits chilling in the cold climate of Skyrim are almost completely eliminated. The armors can be improved at a workbench, but they cannot be crafted or bought.

# In-Game MCM Options

Everything not listed below is already configured for you. Feel free to peruse the settings and change them as you like.

**Wait until no new messages appear in the top left corner!**

I recommend starting by configuring ALL of your MCM menus EXCEPT for Skyrim Unbound. Once this is done open the console by pressing the grave ( ` ) key and typing 'save configured' Assuming you haven't made load order changes that break your saves then the next time you start a new character you can, from the main menu, open the console and type 'load configured' to start a new character without having to do all of your MCM choices again...

If it's not listed below then either the defaults are good enough (TUDM stamina costs for instance) or it's totally up to user preference. Work through all of the menus mentioned below while additionally customizing anything else as you see fit. Once that's done open up the 'Skyrim Unbound' MCM menu to choose your starting options...

In order to experience all of the GAT + Hyrule content I highly recommend that you start as a dragonborn character.

Either click 'Begin Your Adventure' or close the MCM menus and hit the 'enter' key to begin character creation.

## CGO

- Unlocked Grip
  - NPCs Change Grip [ ]

- Dual Wield Blocking
  - Hotkey (Anything you like)

- Leaning
  - Lean Multiplier (1st Person) 0.25 (Any value is fine)
  - Lean Multiplier (3rd Person) 0.25 (Any value is fine)
 

## Immersive HUD

- Key Press Toggles [x]


## Sky UI

- Advanced
  - SWF Version Checking
  - Map Menu [ ]

## Skyrim Unbound Reborn
This is the alternate start mod used by this list and you configure it while floating above Helgen after starting a new game. Set Dragon Souls based on if you want to be the Dragonborn or not, dragon delay based on how you want the game to determine when dragons should spawn, etc. 
  To quickly set the type of starting equipment you have, click presets and select one of the options. You will be told what you'll start with. This is separate from where you'll start. 
  
Once configured, you can exit out of pause menus and press Enter to move on to the game. 

## Sneaking and controllers

- If using a controller go into the MCM for The Ultimate Dodge Mod, enable gamepad compatibility and select sneak style 1 or 2. Sneak Style one is that the sneak button dodges when a weapon is drawn and sneaks when one isn't drawn. Two is that it sneaks if you press it while not moving and dodges if you press it while moving.


# Character Creation

Using [RaceMenu](https://www.nexusmods.com/skyrimspecialedition/mods/19080) you can create a stunning looking character.

RGE currently ships with a preset for the Nord Female that makes your character resemble Linkle from Hyrule Warriors.

# Getting Started in Game

The Relics of Hyrule content is very much explore and figure it out. There are no quests or markers to lead you on your way. Keep an eye and an ear open for glowing fairies and tinkling noises as those mark most locations of Hyrule content. You can find an initial piece of content in Riverwood near the bridge that Faendal paths across to chop wood.

The GAT content is woven into the main game. The imperial forces will be contesting you for everything including much of the major Hyrule content. At some point you will want to join the Chiss Resistance. While there are many ways to do this an easy one is to head towards Bleak Falls Barrow and stop at Riverwood's Folly to chat with the resistance members there about joining. I advise against actually doing anything with BFB until you've joined the resistance and they ask you to do so.

You may want to keep a companion or two with you at all times as GAT is balanced around having a squad. All vanilla followers have been significantly upgraded via 'Special Edition Followers'. Additionally I've included a funny old wizard 'Benjamin Doon', a nordic battle maid 'Danika', a vampire lord 'The Pale Lord', an awesome lich 'Daanik', our favorite blue cat Inigo, and last but not least Lucien. GAT itself comes with around thirty followers that you can recruit into your squad as well.

As configured by default your sneak key is ctrl, your dodge key is space and your shift key is jump. If you want to change this then go into the MAIN settings then controls then set the SNEAK key to whatever you want your DODGE to be. Then setup your jump to whatever it should be. Finally go into the MCM section for 'The Ultimate Dodge Mod' and set the sneak key to whatever you want to actually sneak with.

Spell Siphon is included in this modlist. It's an amazing way to play any mage/spellsword/arcane archer type character but it takes a bit of getting used to. If you want to make use of this feature then read the 'Spell Siphon' book in your inventory to kick things off. The payoff is huuuuuge.

Have fun!

# FAQ

- I play on 21:9 resolution but the UI looks weird?
  - Search `21x9` in MO2 then enable all of them.
- I'm on a controller and the controls are weird?/I want to play on a Controller
  - To enable controller support, open MO2's INI editor for Skyrimprefs.ini and change bGamepadEnable=0 to bGamepadEnable=1. 
  - Disable `Better Container Controls` if the controls feel weird.
  - Reference [The Ultimate Control Scheme](https://www.nexusmods.com/skyrimspecialedition/mods/29381) for controller layout.
  - Due to TUDM only supporting 4way dodging on gamepad we use [antimicro](https://sourceforge.net/projects/antimicro.mirror/) to enable 8way dodging.  Download it and [setup your left stick to output WASD](https://i.imgur.com/hSgdwQc.png).
  - Alternatively... disable the `RGE - Controlmap` mod and reset your controls in the main skyrim controls menu then configure everything as you like from scratch.
- My character is stuck dodging
  - This happens occasionally on load but rarely in gameplay. Press 'G' to fix it.
- Spellsiphon looks pretty complicated, could you describe the basics?
  - Basically when you use the new Bind shout from the Spellsiphon book, you equip the new spells draw and ward. Ward acts as a light, a shield in combat, and a healing spell. Draw acts as your offensive spell and does a small amount of damage. After using it on something for a short time, it changes to 1 of 3 spells depending on what you used it on. Living things (and constructs) give you the Life element spell that does lightning damage, corpses give you Death element that does cold damage, and everything else gives World, which does fire damage. By swapping between elements as you go you build up a buff that increases damage done. These are the basics.
  - [Th Spellsiphon manual](https://docs.google.com/document/d/18Y3fjwNQ8t0uAIkr4fuH0CLliyindpO3LEResV4I9PM/edit) does an excelent job explaining the exact mechanics in more detail and there is in an ingame tutorial for it as well. 
- Why am I floating over Helgen after hitting new game?
  - This is the start of the mod Skyrim Unbound Reborn. Open the main menu and go to the MCM settings for it and you can set things like where you'll start, what items you start with, your starting spells, etc. Of specific note is the Dragon Souls option. Set this to Dragonborn if you want to be the dragonborn and get dragon souls from killing them.
- Where are the dragons?
  - By default they're on a delay of 7 to 21 ingame days. You can customize that in the Skyrim Unbound MCM.
- How do I start Invasion of Skyrim?
  - Talk to resistance members and ask to join, you'll be invited to their base at level 15.
- How do I start the main story of Skyrim?
  - To start the main story kill and absorb the soul of your first dragon. Should you not have set the Dragonsouls option to Dragonborn as told to in the readme, go to the Skyrim Unbound Reborn MCM. Enable the Debug Mode (on the last MCM page) and use the Dragon Souls option and change it to Dragonborn.. Then disable the Debug Mode again. You can tell if this needs to be done by seeing if you absorb a soul from the first dragon you kill.  
- I have strange striped shadows on stuff or deep shadows on faces!
  - If you experience strange shadows on character faces or other things, turn off bSAOEnable=1 in the SkyrimPrefs.ini file in your RGE install's profiles folder.  Alternatively, you can also find MO2's ini editor in the dropdown list that looks like puzzle pieces and use that to change it. Or go to the tools folder of your install and run BethINI while MO2 is closed and change it there.

# Tweaking Performance

My Setup:

- Ryzen 3700x
- 1080 ti
- 32GB DDR4-3200 RAM (CL 14)
- Game and MO2 running on an M.2 NVME SSD

## Tweaking the ENB

This should always be the first thing you tweak. Disabling the ENB entirely can give you anything from 20 to >70 FPS. The ENB this Modlist comes with (see [Audio and Weather](#audio-and-weather)) is rather performance intensive. Open the ENB GUI using `Right Shift + Enter` (`Right Shift` is under the `Enter` key). This will open up the ENB GUI where you can enable and disable certain effects in the left panel.

- `Bloom`: Can give you up to 3 FPS, will make light sources less bright
- `DepthOfField`: Can give you up to 10 FPS, disabled by default and not really suited for gameplay
- `Distant/DetailedShadow`: Those two can really give you a lot of FPS back depending on your shader settings (game settings). They are very noticeable.
- `ComplexFire/ParticleLights`: You won't see a lot of difference at first when disabling those two, but when particles are on screen (eg using magic or near light sources such as fires), they can _burn_ through your FPS

## Tweaking the Game Settings

I highly recommend using [BethINI](https://www.nexusmods.com/skyrimspecialedition/mods/4875) which is included in this Modlist (can be found in `MO2/tools/BethINI`). I recommend tweaking the `Detail` section for more FPS:

- `Shadow Resolution`: Very big one. A good balance is `2048` which is the borderline between high FPS drainage and garbage looking shadows.
- `Ambient Occlusion`: Highly recommended to leave this at `None`. The ENB this Modlist comes with, uses the ENB SAO which is 10x better and performance friendly than base game SAO. This is the source of strange shadows mentioned in the FAQ.
- `Detailed Draw Distance`: Maybe try `2000` instead of `2800` but you won't notice a lot of FPS gain (maybe 1-3)
- `Remove Shadows`: If you really struggle, use this. This will disable all Shadows (not recommended)

If you experience strange shadows on character faces, turn off bSAOEnable=1 in the SkyrimPrefs.ini file in your RGE install's profiles folder.  Alternatively, you can also find MO2's ini editor in the dropdown window that looks like puzzle pieces and use that to change it. Or go to the tools folder of your install and run BethINI while MO2 is closed and change it there.

This setting may change if you use BethINI to change your settings to one of its presets to try and get better performance.

To make changes such as switching from borderless windowed mode to exclusive full screen, edit the SSEDisplayTweaks.ini file in (RGEInstall Folder)\mods\RGE - Patches\SKSE\Plugins. This overrides the one in the SSE Display Tweaks folder. 


# Removing the Modlist

You can just remove the MO2 folder and be done with it. 


# Credits and Thanks

- _YOU_ for actually reading the readme. Thanks a ton!!
- The Phoenix Flavor by Phoenix - General ideas and awesomesauce derived therefrom
- Lotus by erri120 - README format and NPC visuals
- Total - Being a really helpful guy.
- Halgari and everyone the WJ Team - Wabbajack is awesome and so are you
- Frenchy - Thanks for the great work on the Linkle preset!
- Forgotten God and Frenchy - Thanks for the great work on the logo and main menu replacer!!
- Cal - For providing his Collision Optimization mod to help fix performance issues when looking at specific objects.


# Contact

While I'm always available on the [Animonculory Discord](https://discord.gg/theanimonculory), I would advise checking the [Issues](https://github.com/lexcia98/rge/issues) (open **and** closed ones) on GitHub first if you have any problems. The same goes for _Enhancements_ or _Feature/Mod Requests_. **DO NOT DM ME ON DISCORD. I WILL NOT PROVIDE SUPPORT FOR YOU IN DMS**.

# Contributing

See [Contributing](CONTRIBUTING.md).

# Changelog

See [Changelog](CHANGELOG.md).
