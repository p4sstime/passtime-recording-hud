![logo](https://i.imgur.com/HVyxIC3.png)

<div align="center">

This is a modified version of m0rehud classic (pulled 4/28/24) to be a good option for recording PASS Time demos. This HUD is designed to only have HP, ammo, and the PASS INCOMING indicator. No killfeed, no damage indicators, nothing else.

Recommended commands to run this with:\
```
hud_deathnotice_time 0                // disable kill feed
hud_saytext_time 0                    // disable text chat
cl_hud_killstreak_display_alpha 0     // disable killstreak notices
hud_combattext 0                      // disable damage numbers
tf_use_match_hud 0                    // disable match status
cl_hud_playerclass_use_playermodel 0  // disable hud player models
tf_passtime_player_reticles_friends 0 // disable passtime team icons
tf_passtime_player_reticles_enemies 0 // disable passtime enemy icons
```
Copy-pasteable version:\
```hud_combattext 0;cl_hud_killstreak_display_alpha 0;hud_saytext_time 0;hud_deathnotice_time 0;tf_use_match_hud 0;cl_hud_playerclass_use_playermodel 0;tf_passtime_player_reticles_friends 0;tf_passtime_player_reticles_enemies 0```
</div>
