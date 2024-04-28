![logo](https://i.imgur.com/HVyxIC3.png)

<div align="center">

This is a modified version of m0rehud classic (pulled 4/28/24) to be a good option for recording PASS Time demos. This HUD is designed to only have HP, ammo, and the PASS INCOMING indicator. No killfeed, no damage indicators, nothing else.
</div>

You need to name this folder to start with an _. It needs to load before your PASS Time reticle mods get loaded. This only overwrites the circle for your friendly ball carrier, not your actual reticle.

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