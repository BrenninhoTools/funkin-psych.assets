Put your stage .JSON files here

objects: sprite, animatedSprite, square, girlfriend, opponent, boyfriend
prefabs: phillyTrain, mallCrowd, backgroundGirls, backgroundDancer, dadBattleFog, scene3D (see docs/3D.md)
extra object keys: visible, blend, graphicSize, velocity, active, updateHitbox

behaviors: { "on": trigger, conditions..., "actions": [ ... ] }
triggers: create, createPost, update, songStart, countdown, beat, step, section, event, cutscene, endCutscene
conditions: every, offset, chance, cooldown, initialCooldown, songs, notSongs, storyMode, seenCutscene, lowQuality, flashing, camZooms, event, value1, value1Not, nextSong
actions: play, dance, call, sound, music, set, add, tween, color, fade, zoom, cameraZoom, flash, cameraFade, focus, spotlight, hud, cutscene, pause, startCountdown, endSong, defaultZoom, trail, gameOver, precache, stopTweens, play3D
every action accepts "delay" and "when"
values: "$defaultCamZoom", "$value1", "$value2", "$flValue1", "$flValue2", "#RRGGBB"

modules: dadbattleSpotlight, phillyGlow, schoolDialogue, limo, tank, phillyStreets, phillyBlazin
