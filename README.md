![logo](https://i.imgur.com/HVyxIC3.png)

<div align="center">

This is a modified version of m0rehud classic (pulled 4/28/24) to be a good option for recording PASS Time demos. This HUD is designed to only have HP, ammo, and the PASS INCOMING indicator. No killfeed, no damage indicators, nothing else.
</div>

**You need to name this folder to start with an _.** It needs to load before your PASS Time reticle mods get loaded. This only overwrites the circle for your friendly ball carrier, not your actual reticle.

Recommended commands to run this with:
```
hud_deathnotice_time 0                // disable kill feed
hud_saytext_time 0                    // disable text chat
cl_hud_killstreak_display_alpha 0     // disable killstreak notices
hud_combattext 0                      // disable damage numbers
tf_use_match_hud 0                    // disable match status
cl_hud_playerclass_use_playermodel 0  // disable hud player models
tf_passtime_player_reticles_friends 0 // disable passtime team icons
tf_passtime_player_reticles_enemies 0 // disable passtime enemy icons
crosshair 0                           // disable crosshair
cl_use_tournament_specgui 0           // disable spectator hud
cl_spec_carrieditems 0                // disable carried items showing when spectating players
glow_outline_effect_enable 0          // disable glowing outline effect around dropped weapons
```
These are included in the cfg of the files. Just run `exec pass_record` to run the above commands.

If you want to reset these commands back to defaults (except for one; cl_use_tournament_specgui is 0 by default), just run `exec pass_stop` when you're done.

### Disabling Additional HUD Elements

If you want to disable health, ammo, or the PASS INCOMING indicator, here's how to do it.

For health, go to `resource\ui\hudplayerhealth.res` and change line 12 `visible` to 0.

For ammo, go to `scripts\hudlayout.res` and change line 23 `tall` to 0.

For PASS INCOMING, go to `resource\ui\hudpasstimepassnotify.res` and change line 23 `tall` to 0.

After making any changes:
- Make sure you have Demo UI open
- Hit the `Reload HUD` button in your main menu or type `hud_reloadscheme` in console
- Your HUD will become extremely cluttered with random elements. This is normal. Resume your demo and the changes should take effect.

### If You're Crashing

Add a `valve.rc` file to `/cfg/`. This'll basically stop your autoexec from loading. For me, this helps with crashes.

Screenshot:
![image](https://github.com/blakeplusplus/passtime-recording-hud/assets/76140847/d35cfa5c-4f6a-4271-8fc1-9e7124394f60)

### Alternatives

One made by Blu2th is available here named [KERMITPASSHUD](https://discord.com/channels/471798073996345344/472303455579406336/1255997570564755456). You need to be in the NA 4v4 PASS Time Discord to access this Discord message.
