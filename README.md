//Autoexec file

//Rates
rate "128000"
cl_cmdrate "128"
cl_updaterate "128"
cl_interp "0.0"
cl_interp_ratio "1.0"
cl_lagcompensation "1"


//Audio
volume "0.4"
voice_enable "1"
voice_scale "1.0"
windows_speaker_config "1"
snd_musicvolume "0.0"
snd_mixahead "0.05"
snd_headphone_pan_exponent "2"
snd_headphone_pan_radial_weight "2"
snd_legacy_surround "0"
snd_mute_losefocus "1"
lobby_voice_chat_enabled "0"


//Video
mat_monitorgamma "2.1"
fps_max "145"
fps_max_menu "60"
r_dynamic "0"
r_drawtracers_firstperson "0"


//Mouse
zoom_sensitivity_ratio_mouse "1.0"
m_rawinput "1"
m_customaccel "0.0"


//Misc
developer "0"
con_enable "1"
con_filter_enable "2"
con_filter_text "Damage"
con_filter_text_out "Player:"
ui_steam_overlay_notification_position "bottomright"
player_nevershow_communityservermessage "1"
mm_dedicated_search_maxping "100"
gameinstructor_enable "0"
option_duck_method "0"
option_speed_method "0"
cl_forcepreload "1"
cl_downloadfilter "none"
cl_disablehtmlmotd "1"
cl_autohelp "0"
cl_showhelp "0"
cl_disablefreezecam "1"
cl_teammate_colors_show "1"
cl_loadout_colorweaponnames "1"
cl_autowepswitch "0"
cl_use_opens_buy_menu "0"
closeonbuy "0"
hud_takesshots "0"


//HUD
hud_scaling "0.8"
hud_showtargetid "1"
cl_draw_only_deathnotices "0"
cl_righthand "1"
cl_showloadout "1"
cl_showpos "0"
cl_showfps "0"
cl_hud_healthammo_style "0"
cl_hud_background_alpha "0.5"
cl_hud_color "0"
cl_hud_playercount_showcount "0"
cl_hud_playercount_pos "0"
viewmodel_presetpos "0"
viewmodel_fov "68"
viewmodel_offset_x "2.5"
viewmodel_offset_y "2.5"
viewmodel_offset_z "-2.0"
cl_viewmodel_shift_left_amt "0.5"6
cl_viewmodel_shift_right_amt "0.25"
cl_bobcycle "0.98"
cl_bob_lower_amt "5"
cl_bobamt_lat "0.1"
cl_bobamt_vert "0.1"


//Keybinds
bind "kp_pgup" " buy molotov; buy incgrenade;"
bind "kp_downarrow" " buy smokegrenade;"
bind "kp_pgdn" " buy flashbang;"
bind "kp_uparrow" " buy hegrenade;"
bind "kp_ins" " buy vesthelm; buy vest;"
bind "kp_del" " buy defuser;"
bind "kp_end" "buy ak47; buy m4a1;"
bind "kp_leftarrow" "buy mac10; buy mp9;"
bind "kp_5" "buy awp;"
bind "kp_rightarrow" "buy p250;"
bind "kp_home" " buy taser;"


# Drop bomb
bind n “use weapon_knife; use weapon_c4; drop; slot1”

# Increase Volume When Walking
alias +walkvol "incrementvar volume 0 1 0.5;+speed"
alias -walkvol "incrementvar volume 0 1 -0.5;-speed"
bind shift +walkvol

# Show net_graph
net_graph "1"
net_graphheight "9999"
bind "TAB" "+scorenet"
alias "+scorenet" "+showscores; net_graphheight 0"
alias "-scorenet" "-showscores; net_graphheight 9999"

# Quickswitch
alias +knife slot3
alias -knife lastinv
bind q +knife

# Mute all
bindtoggle j voice_enable

# Nades
bind mouse4 "use weapon_flashbang";
bind mouse5 "use weapon_smokegrenade";
bind x "use weapon_hegrenade";
bind t "use weapon_molotov;use weapon_incgrenade"

# Find bomb
alias "+use_radar" "+use; cl_radar_always_centered 1; cl_radar_scale 0.8; gameinstructor_enable 1"
alias "-use_radar" "-use; cl_radar_always_centered 0; cl_radar_scale 0.4; gameinstructor_enable 0"
bind "e" "+use_radar"


bind uparrow "incrementvar volume 0.0 1.0 0.05"
bind downarrow "incrementvar volume 0.0 1.0 -0.05"
bind rightarrow "ignoremsg"
bind leftarrow "ignorerad"

# Use voice chat
bind "v" "+voicerecord"


//Radar
cl_radar_always_centered "1"
cl_radar_rotate "0"
cl_radar_scale "0.4"
cl_radar_icon_scale_min "0.4"


//Crosshair 
cl_crosshairstyle "4";
cl_crosshaircolor "1";
cl_crosshairsize "1.9";
cl_crosshairgap "-2";
cl_crosshairalpha "200";
cl_crosshairusealpha "1";
cl_crosshairthickness "0";
cl_crosshaircolor_r "219";
cl_crosshaircolor_g "14";
cl_crosshaircolor_b "33";
cl_crosshair_drawoutline "1";
cl_crosshair_outlinethickness "1.1";
cl_crosshairdot "0";
cl_crosshair_t "1";
cl_crosshairgap_useweaponvalue "0";
hud_showtargetid "1";

//Custom
mm_dedicated_search_maxping 25
dsp_slow_cpu 0 // High quality sound

# Write to standrd config.cfg
# host_writeconfig
