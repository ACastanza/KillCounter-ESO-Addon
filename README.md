# KillCounter ESO Addon

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
