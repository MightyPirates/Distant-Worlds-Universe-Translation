Distant Worlds - Universe
Read me File – 28 Novemeber 2014
Version 1.9.5.10BETA
	
Welcome.

Thank you for playing Distant Worlds - Universe™!  We are always looking for ways to improve your gaming experience.  For the latest information on the game, please go to the Matrix Games web site at www.matrixgames.com.

Below you will find the latest and greatest information on Distant Worlds - Universe™.  Information in this document supersedes that in the official game manual.


Troubleshooting:

Ensure that your system meets the minimum system requirements.  These are found in the game manual.  Also, ensure that you have the latest video and sound drivers available for your system and that you have upgraded to the latest versions of XNA Framework and .Net Framework from Microsoft.  The vast majority of reported problems are resolved by upgrading all drivers, XNA Framework and .Net Framework to the latest versions.  

If you are still experiencing problems with the game, please use our Help Desk at www.matrixgames.com/helpdesk or post in the Distant Worlds - Universe™ Support Forum at www.matrixgames.com.  Please provide as much detail on your issue as you can.
To obtain optimum game performance, close all other applications before beginning a game. 

Change History:
V1.9.5.10BETA – Novemeber 28, 2014
BUG FIXES
bases built at planets/moons/asteroids no longer detach when built by improvised construction ships (e.g. Exploration ships) that use a subrole other than 'Construction Ship'
ship captain characters now have their skills and traits revealed after their first battle
PIRATES
pirate bases with Gravity Well Projectors will now properly stop all enemy ships, not just other pirates
pirate income from controlled colonies is now never negative, even when colony has negative revenue (i.e. colony maintenance upkeep greater than income)
maintenance costs for each troop unit now properly shown in Troops screen when playing as pirate
in pirate missions panel in Empire Navigation Tool, now properly show Defend missions when "Showing Available Missions" and "Showing All Missions Types" (when playing as pirate)
pirate factions now properly process *owned* colonies so that the following activities occur: troops recruited, population growth rates vary, luxury resources ordered, population race bonuses applied, etc
pirate resort bases now properly cleaned up when destroyed
OTHER
Ships and Bases screen now remembers last filter setting
added troop strength summary to hover tip in Selection Panel when Colony selected and hovering mouse over 'Troops' line

V1.9.5.8– September 8, 2014

CRASH FIXES 
fixed rare crash when detect pirate smuggler docking at base 

fixed rare crash when ships in combat 

BUG FIXES 
fixed bug where race-specific diplomacy mood music was not working in a theme 

SHIP DESIGN 
AI ship design process now automatically adds extra energy collector components to match static energy requirements of design (similar to the way reactors are added) 
AI ship design now increases size of Carrier designs (beyond default design template) when construction size allows (like Capital Ships already did) 
added medium and large freighter designs to AI ship design shrinking process (attempt to fit within current maximum construction size) 
fighter firepower now listed in ship design detail screen (Weapons panel), to allow better comparison of military designs (firepower and fighters listed separately) 

MODDING 
 now optionally allow setting battle tactics, invasion tactics and fleeWhen settings for designs in design template files. To do this, for any design template file for any race, use the following entries (Entry name with possible values after the colon): 
TacticsWeaker: Evade, Standoff, AllWeapons, PointBlank 
TacticsStronger: Evade, Standoff, AllWeapons, PointBlank 
TacticsInvasion: DoNotInvade, InvadeWhenClear, InvadeImmediately 
FleeWhen: EnemyMilitarySighted, Attacked, Shields50, Shields20, Never 

OTHER 
increased hold-off range for tractor beams on spaceports against enemy troop transports (i.e. prevent colony invasions) 
increased the maximum per-resource cargo space at spaceports and other bases from 30000 to 120000 
ship decision whether to use tractor beams to pull or push a target now uses optimal attack ranges defined by battle tactics, e.g. when set to Point Blank then will pull within close range, when set to Evade will always push. Spaceports defending a colony will push when enemy troop transport gets too close in an attempt to prevent them from dropping invading troops at the colony 
idle automated AI fleets and troop transports will now unload troops at colonies that have pirate facilities but insufficient troops to clear them 

V1.9.5.7– August 12, 2014

CRASH FIXES 
fixed crash when ship attacks target 
fixed crash when reviewing pirate character traits 
fixed crash when fighter evaluates enemy threats 
fixed crash when empire declares war 
fixed crash when opening Construction Yards screen 
fixed rare crash when applying sun shadow graphics on planets in low-memory conditions 

MODDING 
allow customizing diplomacy mood music to be race-specific (music played when open Diplomatic Contact screen). Will play race-specific music when named race subfolder present under Customization\THEMENAME\sounds\effects (e.g. Customization\MyTheme\sounds\effects\human). Mood music filenames as follows: diplomacyMoodNeutral.mp3, diplomacyMoodAngry.mp3, diplomacyMoodHappy.mp3, diplomacyMoodMenacing.mp3 
increased maximum number of components from 170 to 300 (components.txt) 
added optional ship design template files for planet destroyers in themes. To use, place a custom ship design template named "PlanetDestroyer.txt" in the appropriate race folder 
added new super weapon types, allowing different types of planet destroyer weapons: in addition to the default super beam weapons can now also have super torpedos, super missiles, super rail guns, super phasers. Any of these can be set to be planet destroying weapons when damage is 10,000 or greater (weapon component Value1). Particularly useful in conjunction with new planet destroyer ship design templates mentioned above. To add these new super weapons to a custom theme, use the following values in the components.txt file (Type): 62=SuperTorpedo, 63=SuperMissile, 64=SuperRailGun, 65=SuperPhaser. You can also focus an empire's tech efforts to these new areas using the following new values in the race policy files (ResearchDesignTechFocus1-6): 30=SuperTorpedo, 31=SuperMissile, 32=SuperRailGun, 33=SuperPhaser 

OTHER 
decreased chance of counterintelligence intercepting enemy intelligence missions, especially when targeted enemy agent has high mission skill level (i.e. harder to catch) 
fixed display of game difficulty level in Achievements tab of Empire Comparisons screen (was previously sometimes mislabelling difficulty levels) 
AI ship design now better at shrinking mining ships when maximum construction size is low 
AI ship design now better at shrinking military ships with fighter bays when maximum construction size is low 

V1.9.5.6 – July 18, 2014

BUG FIXES
character energy savings bonuses now properly reduce energy consumption instead of increasing it 

CRASH FIXES
fixed rare crash when drawing ships
fixed crash when giving monetary gifts to other empires
fixed crash when sorting ships in fleets
fixed crash when evaluating designs 

MODDING
allow including GameText.txt from a custom mod (i.e. read from theme folder)
altered images\units\creatures folder to be read from the mod (if present) instead of the root game folder
allow modding MP3 files in sounds\EFFECTS (not just WAV files)
fighters now properly use WeaponImageIndex value in fighters.txt to allow customization of fighter weapon effects
now allow per-race modding for user interface in a theme (add subfolders named by race under images\ui\chrome folder to mod most chrome images, e.g. customization\THEMENAME\images\ui\chrome\human) 
custom characters with '?' appearance order now never appear at game start 

SHIP DESIGN
AI ship design now properly adds damage control components when repair bots are unavailable
further optimized AI ship design process to allow shrinking designs with maximum construction size while still ensuring critical components are present (e.g. weapons on military ships)
Fighter Bay components now considered as weapons in military ship designs (i.e. can have military ship designs with no weapons except for Fighter Bays)

GAME BALANCE
AI now gives higher preference to mining station build locations that are closer to space ports, colonies, etc
strategic resources used in construction (for components) now weighted slightly higher when considering stockpiles at spaceports and elsewhere
counterespionage strength adjusted - slightly less chance of intercepting enemy intelligence missions 
reduced chance of empires switching to Corporate Nationalism government type when available 
altered empire military strength measurement to better account for fighters (affects diplomacy and AI empire evaluations) 
independent colonies now recruit more defending militia troops 

PIRATES
pirate factions now pay maintenance for any non-pirate raider troops (once have proper colonies) 
pirate faction flags retain pirate symbol in top-left corner when edited in game editor 
pirate faction flags properly update in galaxy view when edited in game editor 
pirate factions can now build normal planetary facilities and wonders at fully owned colonies using right-click pop-up menu and action buttons 

OTHER
slightly improved game performance
can now build bases in disputed systems if your empire has a colony in the system

V1.9.5.5 – July 1, 2014

CRASH FIXES 
added extra safeguards to help prevent crashes when using faulty themes 
fixed rare crash when giving diplomatic gifts

BUG FIXES 
now cancel intelligence missions when target colony or base conquered, destroyed, etc 
fixed bug where sometimes getting tech bonuses from disassembling ships without advanced tech 
Ion Defense and Tractor Beams no longer counted as weapons when checking civilian designs in Ship Design editor 
ensure never load pirate raider troops when loading troops onto transports (e.g. loading troops from own colony while attacking pirate base) 
ensure custom planetmaps getting loaded ('other' folder) 
ensure mouse scroll wheel retains focus when Character and Empire Policy screens are closed 
ensure colonies only appear once in Top Colonies screen, even when controlled by pirates 
fixed problem where ships with advanced tech were sometimes not giving tech bonuses when disassembled 

MODDING 
NEW MODDING FEATURE: defined Research path. Optionally allow specifying project order for a race for each tech tree (see new entries in race files: WeaponsResearchProjectOrder, EnergyResearchProjectOrder, HighTechResearchProjectOrder) 
reverted file loading for certain files to be encoding neutral, i.e. does not matter whether ANSI or UTF-8 (resources.txt, components.txt, research.txt) 
increased maximum government amount to 60 (governments.txt) 
increased maximum planetary facility amount to 100 (facilities.txt) 
increased maximum fighter amount to 50 (fighters.txt) 

USER INTERFACE 
increased font sizes for main menu items when screen resolution is greater than 1920x1080 
increased font size for Galactopedia topic index 
increased font size of hover panel at bottom-middle of screen 
increased font size in Game Options screens 
slightly increased font size in main view for system names, nebula names, etc 
increased font size of tradeable items in Diplomacy trade screen 
increased font size in hover tech descriptions in Diplomacy trade screen 
increased font size in Component Guide screen (Design Detail screen and Research screen) 
ensure correct empire remains selected in Diplomacy screen when conclude trade deal 

GAME BALANCE AND AI 
further improved AI ship design: no longer add too many extra reactors, nor remove too many shield components, when attempting to shrink a new design to fit within construction size limits 
increased chance of counterintelligence missions successfully intercepting enemy intelligence missions, especially for agents with high counterintelligence skill levels 
random government selection more balanced (no longer frequently choosing Military Dictatorship) 
initial home system ruins (Age of Shadows) now never contain system map bonuses 
reduced number of spaceports empire builds when has low population 
increased maximum fleet count. Now relates to overall number of ships and bases, up to maximum of 100 fleets 
AI empires now check whether colony is safe to build at prior to initiating research station construction (e.g. check for nearby pirates) 
lowered effectiveness of counterintelligence, now better accounts for duration of intercepted mission (3 months vs one year, etc) 

PIRATES 
ensure pirate smuggling freighters repair at pirate base when damaged 
ensure pirate smuggling freighters retrofit when necessary and able 
empire will not detect and attack pirate smugglers when they are smuggling resources for that empire 
ensure that pirate-owned colonies are included when checking for wonder completion 
pirate factions now get research bonuses from scientists at their bases 
pirate factions can now change their home base to any space port in their empire by selecting new option in right-click pop-up menu 

OTHER 
ensure that new settings and savegame folder locations are properly created (My Documents\My Games\Distant Worlds Universe) 

V1.9.5.4 – June 19, 2014
CRASH FIXES 
fixed rare crash when determining object visibility for an empire 

BUG FIXES 
fixed bug where loading a previously saved game was sometimes auto-switching to default theme, even when default theme was already loaded 
building pirate bases, fortresses and Criminal Network using the Facility dropdown list in the Colonies screen now properly assigns facility ownership to player pirate faction 
now ensure that cost for building pirate Criminal Network is always properly deducted 
now ensure that custom ship names (shipNames.txt) are used for new pirate ships built using the Build Order screen 
fixed bug where ship design images were being rotated when received a popup message about new ship type research breakthrough (e.g. Carriers) 
fixed bug where Robotic Troops (BattleBots from Robotic Troop Foundry) were not getting maintenance reduction bonuses when recruited from action button under Selection Panel 

RESEARCH AND SHIP DESIGN 
AI ship designer now always adds sufficient reactors to ship designs (possibly more than one) to enable hyperdrive to operate at full speed 
AI ship designer now more willing to shrink new designs to fit within current construction size limits, especially when first obtain hyperdrive technology 
altered size of starting Colonization Module component (now 300 instead of 360, updated components.txt) 
NEW MODDING FEATURE: allow restricting any research project to specific races using the new ALLOWED RACES line in the research.txt file (updated header comments of research.txt explains) 
improved AI research pathing to better emphasize tech focuses from empire policy (ResearchDesignTechFocus1-6), while still researching other important techs 
increased research output for lab components by approximately 50% (components.txt and research.txt) 

GAME BALANCE 
Shakturi now have faster construction and lower ship maintenance (updated Shakturi.txt race file) 
Shakturi ship design templates now use more weapons and other components (military ships, medium & large spaceports, defensive bases) 
Shakturi empire policy now builds more large military ships and less small military ships 
reputation gain from attacking pirates is now reduced by 50% 
Robotic Troops are now cheaper to maintain (25% of normal instead of 33%), and now twice as fast to recruit 
empires are now more willing to use excess cash on hand as factor when deciding whether to build new ships (e.g. low or negative cashflow, but large cash reserves on hand), especially when at war 
now much harder to perform intelligence missions against Ancient Guardians (steal maps, tech, etc) 

OTHER 
no longer scrap and rebuild fighters after loading a saved game 
all sound effects (button clicks, etc) are now disabled when effect volume is set to zero in options screen 
savegame and settings folder location is now standardized to "My Documents\My Games\Distant Worlds Universe" (this remains the same across version updates) 
now send a message to an empire when one of their colonies is lost to a pirate faction that builds a Criminal Network there 
immediately update empire list in Diplomacy screen when trade Empire contact (can now immediately see new empire in list) 
V1.9.5.3 – June 12, 2014
CRASH FIXES 
fixed crash when drawing long range scanners in galaxy view 
fixed crash when drawing planet in hover panel 
fixed crash when auto-saving game 
fixed crash when loading game with custom theme from main menu 
fixed crash when drawing Empire Navigation Tool 
fixed crash with advisor message when invading independent colonies 
fixed crash when investigating ruins 
fixed crash when calculating troop strength 
fixed crash when editing ship design 
fixed crash when edit very large stars in game editor 
fixed crash when AI assigns new mining mission 

BUG FIXES 
altered Windows API used for checking mouse location to fix screen scrolling to top-left (thus avoiding bug in Windows Vista 64-bit) 
fixed bases detaching from their parent planet/moon/asteroid when initiate retrofit before they are finished their previous retrofit 
sound volume now properly remembered when load games 
Unload Troops missions are now cancelled when target colony changes ownership (thus avoid unloading troops at enemy colony) 
fixed misleading message when your special forces troops destroy hidden pirate base facility at one of your own colonies 
main view now properly regains focus for mouse scroll-wheel when close Build Order screen 
fixed rare bug with pirate colonies over-ordering construction resources 
fixed display problems with main menu screen in Windows XP 

USER INTERFACE 
enabled scaling of Empire Navigation Tool at screen left - use new size button next to close button in each panel to cycle 3 sizes: normal, large, extra large 

OTHER 
improved how Action buttons (under Selection Panel) determine which mining station design to show (gas vs mineral) when building mining stations at planets/moons/asteroids (better support for custom themes with unusual resource distributions) 


V1.9.5.2 – June 6, 2014
CRASH FIXES 
fixed crash when drawing space monsters ("CheckFixNotInSystem") 
fixed rare crash when drawing ships 
fixed rare crash when drawing Empire Navigation Tool 
fixed rare crashes relating to fleet mission assignment 

BUG FIXES 
altered how keyboard input is read (different Windows API) in attempt to resolve view sometimes moving to top-left 
fixed issue where Steam Achievements were often being set prematurely 
fixed AI empires starting and then quickly ending Trade Sanctions - now always honor minimum time period 
fixed RepairBot components being downgraded to Damage Control by AI ship design (updated fix) 
fixed problems when loading and displaying research information when Windows set to some non-English languages (e.g. Turkish) 
ensured that pirate factions are generated at start of a new game when using an existing galaxy map 
slightly increased size of Tutorial screen to account for larger text 
fixed problem where player colony names were sometimes including blank values (colonynames.txt) 

GENERAL GAME BALANCE 
adjusted default ship design templates for each race: Large Spaceports have more docking bays and construction yards, Mining Stations have more docking bays, shields and weapons 
low colony tax rates do not increase population growth rates as much as previously, but now make colony more attractive migration destination 
civilian ships now ensure they have enough reactors to power hyperdrives at full speed (same as state ships already did) 
Fighters now weighted higher when evaluating strength of potential attack targets 
AI now willing to build more military ships when at war, especially when have large cash reserves and powerful enemies 
AI now more willing to build more research stations at home colony at game start 
AI takes more care to avoid overspending on troops 

EXPLORATION 
Exploration ships now scan for resources more quickly, moving on to next exploration target immediately once resources and ruins investigated 
increased amount of automated Exploration ships that are assigned to simply scout systems for colonization targets and ruins instead of performing full resource scan of system and all resources 

FLEETS 
AI fleets are now better at coordinating multi-fleet attacks within own empire against single enemy target (beyond just coordinated fleet attacks with allies) 
increased ratio of AI-created large fleets versus small strike forces (i.e. more large fleets) 
now properly limit coordinated fleet attacks within own empire only to automated attack fleets (not defense fleets or manually controlled fleets) 

OTHER 
now force immediate update of stardate and cash display when open a new screen, e.g. Empire Summary screen 
possession of an operational planet destroyer negatively affects diplomatic relations with other empires ("We are envious of your huge strength and power") 
games now honor global volume settings for music and effects 
improved display performance for main menu screens (e.g. start new game) 
space monsters now properly attack ships in the Dead Zone 
ships can now properly investigate abandoned bases in the Dead Zone 
V1.9.5.1 – May 28, 2014
CRASH FIXES
Fixed crash in ship design screen when changing image scaling
Fixed crash when generating ship designs
Fixed rare crash in game editor when adding asteroid fields
Fixed rare crash with fleets
Fixed rare crash with processing empire messages
Fixed rare crash when identifying raidable colonies for pirates
BUG FIXES
Steam Achievements fixed, should be working again now!
Manually canceled Deep Cover intelligence missions no longer continue to reveal enemy map for rest of game
Fixed bug with loading troops when first non-garrisoned troop is too big for troop bay
Fixed research and ship designs to not auto-update when edit empire in game editor, unless player has ship design automated
Fixed occasional invisible space monsters
Ensure empires properly cleared when using existing save game as galaxy map for new game
Ensure that ruins with delayed events also getting properly investigated
DISPLAY AND USER INTERFACE
Reviewed all in-game font scaling and anti-aliasing and reworked font support to take newer Windows operating system scaling into account.  Font size and clarity should now be more consistent across all systems.
Enlarged and clarified fonts: Diplomacy screen, scrolling message list, tutorial screen, cash and income display
Added Introductory Game button in Start New Game screen, we recommend this as a first game for all new players
Moved PreWarp tutorial to last based on player feedback
OTHER
Added a way to disable the intro movie in the Startup.ini file in the DW installation folder. This may help with some startup black screen issues by manually disabling the intro movie.
Significant performance improvements
Improved look of in-system background nebula clouds
Pirates retain protection arrangements for minimum period before canceling, this should also help with the pre-warp tutorial
Improved randomness of starting government types in new games (for other empires, when random govt selected)
Increased maximum event delay to 32000 days (from 10000)
V1.9.5.0 – May 23, 2014
Initial Release
