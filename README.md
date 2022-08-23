# Jupiter Hell modding documentation

# Callbacks

## on_action

Called when the entity can act (?)

Applies to: entities

    function ( self, entity, time_passed, last )

time_passed: in-game time since the last call

entity: the entity this object is attached to

## on_activate

"Action" button is used (?)

Applies to: entities (incl. menus in terminal)

    function( self, who, level, param, id )

## on_activate_other

## on_activate_valve

## on_adrenaline

## on_aim

Applies to: entities

    function ( self, entity, target, weapon )

## on_apply_damage

## on_area_damage

## on_attach

## on_attacked

## on_bot_disable

## on_bot_hack

## on_break_stealth

## on_callback

## on_claim_fiends

## on_cleared

Called when the level is cleared (when the level title turns blue)

Applies to: events, …

    function ( self, level )

## on_collide

## on_create

Applies to: everything

## on_create_entity

## on_create_player

## on_critical

## on_damage

## on_detach

## on_die

## on_dropped

## on_end

## on_enter

## on_enter_level

Applies to: events, …

Events:
    function ( self, level, entity, reenter )

Entity:
    function ( self, entity, reenter )

## on_entity

## on_exit

## on_finish

## on_fire

## on_heart

## on_hit

## on_holster

## on_incoming_damage

## on_init

## on_junk

## on_kill

## on_level_up

## on_load

## on_lootbox_open

## on_mortem

## on_move

## on_next

## on_noise

## on_picked_up

## on_pickup

## on_portal

## on_post_command

## on_pre_command

## on_pre_move

## on_proximity

## on_rearm

## on_receive_damage

## on_red_unlock

## on_resource_power

## on_setup

## on_shell_close

## on_shell_open

## on_shot

## on_smoke_screen

## on_spot

## on_station_activate

## on_stats

## on_stealth

## on_switch

## on_terminal_activate

## on_terminal_refresh

## on_tick

## on_timer

## on_unique

## on_update

## on_use

## on_wait

## on_wave_clear

## can_bleed

## can_burn

## can_drop

## can_fail

## can_pick_trait

## can_pickup

## is_cleared

# UI

## ui:activate_terminal

## ui:alert

## ui:alert_clear

## ui:confirm

## ui:dead_alert

## ui:get_target

## ui:get_time_ms

## ui:highlight

## ui:mark_tutorial_done

## ui:post_mortem

## ui:queue_visual_event

## ui:reset_help_overlay

## ui:run_animation

## ui:run_visual_event

## ui:set_achievement

## ui:set_help_overlay

## ui:set_hint

## ui:set_saveable

## ui:set_suppress_voice

## ui:set_target

## ui:spawn_fx

## ui:telegraph

## ui:terminal

## ui:text

# World

## world:activate_blueprint

## world:add_buff

## world:add_experience

## world:add_history

## world:add_journal

## world:add_quest

## world:add_transfer

## world:attach

## world:callback

## world:clear

## world:command

## world:command_coord

## world:command_use

## world:create

## world:create_entity

## world:current_transfer

## world:destroy

## world:detach

## world:equip

## world:flush_destroy

## world:get_attribute_add

## world:get_attribute_mul

## world:get_hid

## world:get_id

## world:get_level

## world:get_name

## world:get_player

## world:get_position

Get the position of an entity.

    local c = world:get_position( e )

## world:get_quest

## world:get_slot

## world:get_target

## world:get_text

## world:get_ticks

## world:get_weapon

## world:get_weapon_by_type

## world:hash

## world:has_item

## world:is_multifiring

## world:is_player_owned

## world:is_state

## world:journal

## world:lua_callback

## world:mark_destroy

## world:next_level

## world:next_scent

## world:play_sound

## world:play_voice

## world:preload

## world:rand2x

## world:raw_equip

## world:remove_from_max_kills

## world:remove_item

## world:remove_items

## world:resolve_hash

## world:set_scent

## world:set_seed

## world:set_state

## world:set_target

## world:set_targetable

## world:set_text

## world:special_cleared

## world:special_visited

## world:stash_item

## world:update_environment

## world:wipe_inventory

# Level

## level:activate

## level:add_entity

## level:apply_damage

## level:around

## level:beings

## level:beings_in_area

## level:beings_in_cone

## level:can_close

## level:can_fire

## level:can_melee

## level:can_move

## level:can_reload

## level:can_see_entity

## level:cdistance

## level:change_state

## level:coords

## level:coord_see_entity

## level:distance

## level:drop_all

## level:drop_coord

## level:drop_entity

## level:drop_item

## level:enemies

## level:entities

## level:entity_find

## level:find_coord

## level:fire

## level:get_area

## level:get_being

## level:get_being_raw

## level:get_cell_flags

## level:get_entity

## level:get_item

## level:get_max_cover

## level:get_nid

## level:get_npc

## level:get_rotation_between

## level:get_summon_coord

## level:hard_place_entity

## level:is_alive

## level:is_shootable

## level:is_visible

## level:melee

## level:next_move_towards

## level:pathfinder_test

## level:pickup

## level:pickup_drop

## level:place_entity

## level:random_coord

## level:raw_get_cell

## level:recursive_entity_find

## level:reload

## level:remove_entity

## level:reveal

## level:rotate_towards

## level:rscan

## level:set_cell

## level:set_cell_flag

## level:set_explored

## level:swap_weapon

## level:targets

## level:try_move

## level:use

# ECS

## ecs:add

## ecs:child

## ecs:children

## ecs:first

## ecs:get

## ecs:parent

## ecs:remove

## ecs:root

# Entity

## entity:attach

## entity:attribute

## entity:child

## entity:equip

## entity:flag

## entity:get_position

## entity:get_slot

## entity:get_weapon

## entity:pickup

## entity:stash_item

# Nova engine

## nova.log

## nova.register_prototype

## nova.register_storage

## nova.require

## nova.warning

# Commands

## COMMAND_ACTIVATE

## COMMAND_DROP

## COMMAND_MOVE

## COMMAND_MOVE_E

## COMMAND_MOVE_F

## COMMAND_MOVE_N

## COMMAND_MOVE_S

## COMMAND_MOVE_W

## COMMAND_PICKUP

## COMMAND_REARM

## COMMAND_RELOAD

## COMMAND_USE

## COMMAND_WAIT

# GTK

## gtk.add_station_list

## gtk.add_station_manufacture

## gtk.can_regenerate

## gtk.get_detonation_position

## gtk.get_event_ui

## gtk.get_weapon_group

## gtk.is_ai_group

## gtk.is_blade

## gtk.is_one_handed_blade

## gtk.is_weapon_group

## gtk.place_flames

## gtk.place_freeze_smoke

## gtk.place_smoke

## gtk.place_smoke_type

## gtk.place_toxic_smoke

## gtk.random_cdir

## gtk.update_cloud

## gtk.upgrade_master

## gtk.upgrade_trait

# AI

## aitk.active_goto

## aitk.active_hunt

## aitk.active_hunt_no_player

## aitk.claim

## aitk.convert

## aitk.disable

## aitk.do_attack

## aitk.do_attack_all

## aitk.do_charged_attack

## aitk.do_dual_mortar_attack

## aitk.do_mortar_attack

## aitk.do_reload

## aitk.enemy

## aitk.evaluate_dir

## aitk.find

## aitk.follow

## aitk.follow_player

## aitk.get_ranged

## aitk.group

## aitk.hunt

## aitk.idle

## aitk.is_enemy

## aitk.neuter

## aitk.on_attacked

## aitk.on_noise

## aitk.pet

## aitk.pick_dir

## aitk.pick_target

## aitk.run_state

## aitk.seek

## aitk.sentry_attack

## aitk.sentry_launcher_attack

## aitk.sentry_repair

## aitk.stagger

## aitk.standard_ai

## aitk.turret_attack

## aitk.turret_idle

## aitk.turret_on_attacked

## aitk.turret_ready

## aitk.wait

## aitk.wait_and_idle

## aitk.wait_and_idle_unless_attacked

