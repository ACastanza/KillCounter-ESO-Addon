# KillCounter ESO Addon

## UPDATE LOG
3.2.3
Fixed a minor mathematical bug.

3.2.2
Added K/D ratio levels in Current Sessions Tab
God Mode (Gold) - 10+K/D
Beast Mode (Orange ) - 5+K/D
Super Mode (Blue) - 2.5+K/D
.7-2.5 Green
between .5-.7 Yellow
below .5 Red
Fixed Misspelling of Daggerfall
Fixed Text Overlap

3.2.1
Fixed a major bug where Sorcerer was reporting as Dragonknight and vice versa.
Updated the KC Stat Bar to update on event instead of after event
Removed VR levels
Fixed blank class by making it say "duel". This is back when KC counted kills outside, but not deaths.
Updated the GUI. Re-did all the icons to make them match their respective tab
Updated the draw line visuals between each line.
Updated the class colors on graphs
Updated the background for information
Updated the stat bar to not have cross colors
Possible Future Updates:
Searching Kills, this is far down the line but still being worked on
Background image changes for the menu
Dueling Mode, being looked into

3.2.0
* Fixed / changed a few kill counter elements
- Kill Counter /kc on stat bar is no longer transparent. This is to help visibility in Cyrodiil and modernize it.
* May add a settings option for this

- Changed the Killers tab so that it no longer displays levels. Levels would require a lot of data updating and not update all old player data so this is removed from the table and added Kills To Them so you can easily view Kills From / To the player in the Killers Table

Bug Fixes
- Potentially fixed stats displaying `T` error in housing.

3.1.5b
* fixed error message
Code:
[LAM2] The panel with id 'KillCounterConfig' was registered before addon loading has completed. This might break the AddOn Settings menu.
3.1.5a
* Added another option in panel to view stats quickly

3.1.5
* Added the start of the Settings->Addon panel, for now this just has a button to open /kc settings
- Added another option in settings to disable kill counter stats bar entirely while in cyrodiil or battlegrounds

Known Issues:
- If you open KC settings through panel initially (without default ways of opening) data may show as T, this will fix itself.

Upcoming (Hopefully - 3.2.0-3.2.5)
- Working on un-embedding settings and moving to the panel. Kill Counter is old, so bare with me as I work through it

3.1.0
* Fixed an issue created in 3.0.1, the queue bar wouldn't have transparency
- Also fixed Stat Breakdown window and changed wording for Total Killers / Total Kills to Total Unique Killers / Total Unique Players Killed. This is so its understanding that its different than your actual overall.

3.0.1
* Dynamically fixed the bar to change size when AP is disabled.
- Fixed several old code left over
- Deleted random numbers throwing errors
- Fixed the issue with KC bar size randomly changing to default, if this issue comes back report it

3.0.0
* Addressed several bugs with kill counter and cleaned up the source code a bit more
- Kill Counter now has the ability to turn off AP on the stat bar. /kc settings Note, we do not force /reloadui, you must do this yourself Turning AP off doesn't shrink the bar. This is just for users who use AP meter. You can simply drag the extra bar off the screen.
- Added /kc help which now displays all the commands for kill counter.
- Changes the visuals on the bar minimally to help readability. This includes extending the bar

Bug Fixes:
- Fixed an issue where /kcreset wouldn't full reset stats (AP and killing streaks)
- Fixed an issue where there was `,` displaying in the stats bar
- Fixed the spacing on the bar for K/D to no longer be K/D:(0/0 :0.0) its now: K/D[0/0 : 0.0]
- Fixed an issue where triple digit kills and 7 digit AP would run off the bar (still testing the 7 digit AP)

Known Issues:
- While in housing /kc stats will display the incorrect information. This has to do with ZOS
- KC star bar make not update instantly for AP or /kcreset. This has to do with API issues, the bar will update, the table updates immediately

Wants (Requested and being worked on, TBD)
- Ability to search kills, killers, killing blows via text option
- Moving /kc settings to the default Settings->Addon location

2.7.6b
* adjusted bar size to 405 from 420 should allow up to triple digits on everything and 7 digits on AP.

2.7.6
* Fixed minor issues
- Fixed the kill counter bar where AP numbers would go over transparency (Note, this makes the bar a little longer)
- Confirmed that killing blows tab is counted, just only updated when logged off
- Cleaned up some code
- Starting storing a future class so data now works when a new class is released
- Fixed overlapping table issue

2.7.5
*Updated API
- No fixes or updates yet

2.7.4
* Fixed the rank 50 issue and more - Special Thanks to Ghostbane, check out AP Meter: https://www.esoui.com/downloads/info1792-APMeter.html
- Fixed an issue where K/D color on current session would show red when over 1.0
- Fixed an issue where AP would not report at level 50+ Alliance rank
- Fixed an issue KD in Current session would be "+3.3203" it now rounds to the nearest 2nd decimal place

-->Known Issue: AP on the status bar may update slow, but it updates. All other areas are not affected.

2.7.3
* Fixed several bugs
- Fixed an issue where current session KDR was showing total kills overall
- Fixed an issue where KDR was negative
- Fixed an issue where Necromancer graph was not displaying on Kills/Deaths
- Fixed an issue where overlapping occurred in GUI
- Fixed an issue where AP on bar would go over the transparency

2.7.1
* Added new class support
- Properly tracks Necromancer class while in Cyro/BGs.
- Disabled Kill Counter outside of Cyrodiil/BG. KC was reporting only wins in duels and never losses. I disabled this
and am looking to eventually track both Kills and Deaths outside.
- LibMenuMap is now back to 1.0 not 2.0
- Fixed an issue where Sorcerer was overlapping data with Necromancer (For % breakdown)

2.3.0 - 2.3.2
* New/Improved Features:
- Proper detection of keep/resource capture data.
- Additional settings to filter the information reported in the chat window.
- Added support for Warden statistics. Old KC data still works. (Wardens were already stored, but not used)
- An additional display element for the current Queue position.
- Added a feature to automatically accept the campaign queue invite.
- Both of the previous features can be disabled
- The UI element is much easier to move than before.
- Changed the small stats display window to be a little better organized.
- Quite a few general code changes, efficiency improvements, code golf, etc


2.2.4
*API Bump

2.2.3
*updated to new version
*fixes issues with new API

2.2.2
*rolled Kill Counter to the latest API version

2.2.1
*Fixed an issue caused my an outdated version of LibMainMenu
*fixed issue with current session KDR difference color code. The color is green when a lot above your KDR, Red when a lot below, and yellow when within 70% (above or below)
*Added current Kills table to current session tab. Note: Known issue with this tab, sometimes it will show an extra death on certain rows/players under certain circumstances.
*Removed all archived Kill Counter versions from before 2015


Update 2.7.0 includes a substantial transformation of your Kill Statistics. If you find your existing history to be of extreme importance to you, then I recommend backing it up just in case (By default the information is located at \Documents\Elder Scrolls Online\live\SavedVariables\Killcounter.lua). I've tested a few languages, and multiple sets of data, but there's always a chance something really screwy exists in your data. If something goes wrong, I'd be glad to help you in the comments.

This updates Kill Counter by Mikethecoder/Drummerx04 to 5.0.5. The update is brought to you by @Casterial.
If you find any issues or bugs please post them in the comments I am still working with it as I have limited Necromancers to test on. More updates to come!

Kill Counter is an add-on that Tracks Kills in PVP and other PVP achievements.
It also has Deathmatch/MOBA style Kill streak alerts (Like "Killing Spree" or "Dominating")
as well as death streaks, and capture streaks (Keeps and resources). Kill Counter
also alerts you when a Keep or resource has been captured (50% full). It features an
unobtrusive GUI element for quick view of your current session kills, deaths, Kill/Death ratio,
and Streaks. Individual kills also have their own alerts, with an added sound for that extra level
of satisfaction! All Alerts are fully customizable and can be toggled on/off via the Kill Counter
settings menu (/kc settings, see below).

The GUI element can be dragged to a different place by clicking and dragging the right half of the display bar.

# Kill Counter also has a Full stats menu which lists has multiple distinct sections
1) Overview :: Overview of all stats (totals, KDR, siege stats, etc).
2) Current Session :: List of earnings, kills, killing blows etc, since the last time you logged out... or crashed.
3) Kill History :: All data on kills and killing blows that wasn't lost to game crashes...
4) Killed By History :: Summary of players that have killed you.
5) Breakdown :: Summations/Averages/Other break downs of your stats.
6) Killing Blow History :: The number of kills achieved with each skill you have used.
7) Settings :: Custom settings window. It was already here so I used it. Eventually, I'll try to move it to the standard location.


Kill Counter has always served as a way to track your overall
performance and your performance against other players, other add-ons
such as Miat's provide far more involved additions to the UI, while KC
tries to be unintrusive.

# New/Improved Features update 2.7.0:
- Necromancer class added to statistics
- Kill Counter is fully disabled outside of Cyrodiil
- Statistics now properly support multiple languages.
[From Drummerx04]
- Kill and Killed by messages now include a player link. Now you can now more easily whisper your opponents, even ones with impossible to type names.
- KC no longer counts extra kills when multiple spells hit at the same time. Each killing blow spell is still recorded and reported, but only 1 KILL is counted. You will probably notice a drop in kills reported per hour, but that's because the kills reported are much closer to being correct.
- Quite a few general code changes, efficiency improvements, code golf, etc


# Slash Commands:
/kcreset - reset the counter. you can also do
/kcreset full to reset all of your stats (including list of killed enemies, total kills, etc)
/kc is a general purpose command with many different functions:
/kc on is to turn on KC menu
/kc off is to turn off KC menu
/kc toggle disabled, outdated
/kc stats to view or hide stats panel
/kc settings to view and enable/disable various parts of Kill Counter
/kcreport - Use to report your Kill Counter stats to chat. See below for full list of options for this but an example would be:
/kcreport g1 --reports to guild one
/kcreport z -- reports to zone
/kcreport s full -- reports to say, and shows full stats
/kc report w @somefriendofyours --reports to someone in a whisper

KC Report slash command information: Please see the Author Portal for information on the /kcreport slash command, and more.

Special thanks to @Cinnanmon_Spider, @ANVALIA, @Hank1997, the NA dueling/PVP legend, and many others for helping to create/update/test Kill Counter in the past years.

Kill Counter is officially under Drummerx04 control, but Casterial is temporarily fixing / updating the addon in his absence. Please give him a follow 

If you have any suggestions or improvements for the addon please drop them in the comment section! Just be gentle!
