# PS3SFV_ISO_Tool
 PS3 ISO Verification tool with SFV support

<img src="https://i.gyazo.com/81efabf07987a8e3e2bfd55a9761a9ee.png">

<a href="https://www.psx-place.com/threads/ps3-iso-verification-sfv.27706/">PSX-Place Discussion</a>

<pre>
Usage:

Select ISO to fill out fields.
Click 'Data Avail: NO' to save Verification Data.
Click Verify to use available Verification Data against selected ISO</pre>

<pre>
Current thinking is have two SFV files per Disc ID, One for entire unencrypted image CRC32, Another for 'Disc Contents' individual file SFV for determining incorrect/modified files.

SFV Files can support comments with ; prefix, Can use fields there to store 'Game Title', 'FW Version' and a few other things
</pre>

Example SFV

BLUS31426-IMAGE.SFV

<pre>
;TITLE=Minecraft: PlayStation®3 Edition
;DISCID=BLUS31426
Minecraft_PlayStation3_Edition_BLUS31426_USA_PS3iSO-VERiTAS.iso 5E870047</pre>

BLUS31426-CONTENTS.SFV

<pre>
PS3_DISC.SFB 9F8EF69F
PS3_GAME\ICON0.PNG 5B357D58
PS3_GAME\PARAM.SFO 491BA681
PS3_GAME\PIC1.PNG 2584A393
PS3_GAME\PS3LOGO.DAT EC395C50
PS3_GAME\SND0.AT3 211DE6BE
PS3_GAME\LICDIR\LIC.DAT 4A09406A
PS3_GAME\TROPDIR\NPWR05636_00\TROPHY.TRP AABA28FE
PS3_GAME\USRDIR\EBOOT.BIN 062EE996
PS3_GAME\USRDIR\Common\Media\MediaPS3.arc 16E1FB00
PS3_GAME\USRDIR\Common\Media\font\Mojangles.ttf D9A71739
PS3_GAME\USRDIR\Common\Media\font\CHT\DFTT_R5.TTC DA174805
PS3_GAME\USRDIR\Common\Media\font\JPN\DF-DotDotGothic16.ttf B3BEC10E
PS3_GAME\USRDIR\Common\Media\font\KOR\candadite2.ttf CEC4D7AE
PS3_GAME\USRDIR\Common\Media\font\RU\SpaceMace.ttf 250BC33C
PS3_GAME\USRDIR\Common\res\pack.png B26843D3
PS3_GAME\USRDIR\Common\res\particles.png 62B62C85
PS3_GAME\USRDIR\Common\res\terrain.png A27C8DC3
PS3_GAME\USRDIR\Common\res\1_2_2\pack.png B26843D3
PS3_GAME\USRDIR\Common\res\1_2_2\pack.txt 396ED525
PS3_GAME\USRDIR\Common\res\1_2_2\particles.png CCE6C8B2
PS3_GAME\USRDIR\Common\res\1_2_2\terrain.png CFD025A3
PS3_GAME\USRDIR\Common\res\1_2_2\achievement\bg.png A3AA7039
PS3_GAME\USRDIR\Common\res\1_2_2\achievement\icons.png 46134910
PS3_GAME\USRDIR\Common\res\1_2_2\armor\chain_1.png 98551179
PS3_GAME\USRDIR\Common\res\1_2_2\armor\chain_2.png D27DF6E7
PS3_GAME\USRDIR\Common\res\1_2_2\armor\cloth_1.png AB3306D9
PS3_GAME\USRDIR\Common\res\1_2_2\armor\cloth_2.png E560FD10
PS3_GAME\USRDIR\Common\res\1_2_2\armor\diamond_1.png 0313AEB4
PS3_GAME\USRDIR\Common\res\1_2_2\armor\diamond_2.png 566DF1DA
PS3_GAME\USRDIR\Common\res\1_2_2\armor\gold_1.png E4811C8C
PS3_GAME\USRDIR\Common\res\1_2_2\armor\gold_2.png 3F85A327
PS3_GAME\USRDIR\Common\res\1_2_2\armor\iron_1.png 0DED88AC
PS3_GAME\USRDIR\Common\res\1_2_2\armor\iron_2.png 3EAE0ADE
PS3_GAME\USRDIR\Common\res\1_2_2\armor\power.png F18ECD39
PS3_GAME\USRDIR\Common\res\1_2_2\art\kz.png B96D9B29
PS3_GAME\USRDIR\Common\res\1_2_2\environment\clouds.png 17D31A1B
PS3_GAME\USRDIR\Common\res\1_2_2\environment\light_normal.png C7B10342
PS3_GAME\USRDIR\Common\res\1_2_2\environment\rain.png BE2DA7C6
PS3_GAME\USRDIR\Common\res\1_2_2\environment\snow.png B59E9841
PS3_GAME\USRDIR\Common\res\1_2_2\font\alternate.png 3CE77F99
PS3_GAME\USRDIR\Common\res\1_2_2\font\default.png E723E088
PS3_GAME\USRDIR\Common\res\1_2_2\gui\alchemy.png 7B19C064
PS3_GAME\USRDIR\Common\res\1_2_2\gui\allitems.png D5D54920
PS3_GAME\USRDIR\Common\res\1_2_2\gui\background.png 3935ABCF
PS3_GAME\USRDIR\Common\res\1_2_2\gui\container.png B159E8A1
PS3_GAME\USRDIR\Common\res\1_2_2\gui\crafting.png 321C5410
PS3_GAME\USRDIR\Common\res\1_2_2\gui\crash_logo.png 4E034B73
PS3_GAME\USRDIR\Common\res\1_2_2\gui\enchant.png 4B68AE32
PS3_GAME\USRDIR\Common\res\1_2_2\gui\furnace.png A3B7C88D
PS3_GAME\USRDIR\Common\res\1_2_2\gui\gui.png 7CC724C5
PS3_GAME\USRDIR\Common\res\1_2_2\gui\icons.png EA5541A8
PS3_GAME\USRDIR\Common\res\1_2_2\gui\inventory.png 2FAE1BCB
PS3_GAME\USRDIR\Common\res\1_2_2\gui\items.png 2D990CFF
PS3_GAME\USRDIR\Common\res\1_2_2\gui\particles.png E0B9D0BF
PS3_GAME\USRDIR\Common\res\1_2_2\gui\slot.png 484C235F
PS3_GAME\USRDIR\Common\res\1_2_2\gui\trap.png 6443CB39
PS3_GAME\USRDIR\Common\res\1_2_2\gui\unknown_pack.png A36DB965
PS3_GAME\USRDIR\Common\res\1_2_2\item\arrows.png 77DEFE50
PS3_GAME\USRDIR\Common\res\1_2_2\item\boat.png 519215DA
PS3_GAME\USRDIR\Common\res\1_2_2\item\book.png 9ED9979B
PS3_GAME\USRDIR\Common\res\1_2_2\item\cart.png C90B4B14
PS3_GAME\USRDIR\Common\res\1_2_2\item\chest.png 7037D5A5
PS3_GAME\USRDIR\Common\res\1_2_2\item\door.png 5CF8128D
PS3_GAME\USRDIR\Common\res\1_2_2\item\largechest.png 6699BB37
PS3_GAME\USRDIR\Common\res\1_2_2\item\sign.png 979C0F4D
PS3_GAME\USRDIR\Common\res\1_2_2\item\xporb.png 7BC31CDB
PS3_GAME\USRDIR\Common\res\1_2_2\misc\dial.png 4AB6FC2D
PS3_GAME\USRDIR\Common\res\1_2_2\misc\explosion.png B308AE0A
PS3_GAME\USRDIR\Common\res\1_2_2\misc\foliagecolor.png 063E03DD
PS3_GAME\USRDIR\Common\res\1_2_2\misc\footprint.png 766E87D3
PS3_GAME\USRDIR\Common\res\1_2_2\misc\glint.png 2BB4663D
PS3_GAME\USRDIR\Common\res\1_2_2\misc\grasscolor.png A3698A73
PS3_GAME\USRDIR\Common\res\1_2_2\misc\mapbg.png 8B904CD3
PS3_GAME\USRDIR\Common\res\1_2_2\misc\mapicons.png B5EFAA73
PS3_GAME\USRDIR\Common\res\1_2_2\misc\particlefield.png D965C89A
PS3_GAME\USRDIR\Common\res\1_2_2\misc\pumpkinblur.png 71DD2F56
PS3_GAME\USRDIR\Common\res\1_2_2\misc\shadow.png B4CFA661
PS3_GAME\USRDIR\Common\res\1_2_2\misc\tunnel.png 20110219
PS3_GAME\USRDIR\Common\res\1_2_2\misc\vignette.png 3B1BD1FE
PS3_GAME\USRDIR\Common\res\1_2_2\misc\water.png 51F80181
PS3_GAME\USRDIR\Common\res\1_2_2\misc\watercolor.png 7E117EF5
PS3_GAME\USRDIR\Common\res\1_2_2\mob\cat_black.png 1EA0A5E8
PS3_GAME\USRDIR\Common\res\1_2_2\mob\cat_red.png EEAAD3BF
PS3_GAME\USRDIR\Common\res\1_2_2\mob\cat_siamese.png 2797D9A1
PS3_GAME\USRDIR\Common\res\1_2_2\mob\cavespider.png F56A53D1
PS3_GAME\USRDIR\Common\res\1_2_2\mob\char.png D413391E
PS3_GAME\USRDIR\Common\res\1_2_2\mob\chicken.png B1520BEF
PS3_GAME\USRDIR\Common\res\1_2_2\mob\cow.png A7D9F247
PS3_GAME\USRDIR\Common\res\1_2_2\mob\creeper.png C43EF4C7
PS3_GAME\USRDIR\Common\res\1_2_2\mob\enderman.png 3CB12474
PS3_GAME\USRDIR\Common\res\1_2_2\mob\enderman_eyes.png E970BAC3
PS3_GAME\USRDIR\Common\res\1_2_2\mob\fire.png 3ED7809F
PS3_GAME\USRDIR\Common\res\1_2_2\mob\ghast.png 987C4E4C
PS3_GAME\USRDIR\Common\res\1_2_2\mob\ghast_fire.png A35C999C
PS3_GAME\USRDIR\Common\res\1_2_2\mob\lava.png AB50BDE9
PS3_GAME\USRDIR\Common\res\1_2_2\mob\ozelot.png 0A26BEFF
PS3_GAME\USRDIR\Common\res\1_2_2\mob\pig.png DFE674FA
PS3_GAME\USRDIR\Common\res\1_2_2\mob\pigman.png 50143A85
PS3_GAME\USRDIR\Common\res\1_2_2\mob\pigzombie.png CC98A297
PS3_GAME\USRDIR\Common\res\1_2_2\mob\redcow.png 332EBC1C
PS3_GAME\USRDIR\Common\res\1_2_2\mob\saddle.png D90F1367
PS3_GAME\USRDIR\Common\res\1_2_2\mob\sheep.png 268418C8
PS3_GAME\USRDIR\Common\res\1_2_2\mob\sheep_fur.png 4A5064B6
PS3_GAME\USRDIR\Common\res\1_2_2\mob\silverfish.png FE4F4B9A
PS3_GAME\USRDIR\Common\res\1_2_2\mob\skeleton.png EADAC7FD
PS3_GAME\USRDIR\Common\res\1_2_2\mob\slime.png A27DA092
PS3_GAME\USRDIR\Common\res\1_2_2\mob\snowman.png 0B83F50C
PS3_GAME\USRDIR\Common\res\1_2_2\mob\spider.png 5963D360
PS3_GAME\USRDIR\Common\res\1_2_2\mob\spider_eyes.png 7A366D75
PS3_GAME\USRDIR\Common\res\1_2_2\mob\squid.png 9828FC11
PS3_GAME\USRDIR\Common\res\1_2_2\mob\villager.png 61FE5C56
PS3_GAME\USRDIR\Common\res\1_2_2\mob\villager_golem.png 6DE062B2
PS3_GAME\USRDIR\Common\res\1_2_2\mob\wolf.png 08948458
PS3_GAME\USRDIR\Common\res\1_2_2\mob\wolf_angry.png 156D783E
PS3_GAME\USRDIR\Common\res\1_2_2\mob\wolf_tame.png A5476E9D
PS3_GAME\USRDIR\Common\res\1_2_2\mob\zombie.png 2FF1C947
PS3_GAME\USRDIR\Common\res\1_2_2\mob\enderdragon\beam.png 0DE51C94
PS3_GAME\USRDIR\Common\res\1_2_2\mob\enderdragon\body.png 87BDDFDF
PS3_GAME\USRDIR\Common\res\1_2_2\mob\enderdragon\crystal.png 36ED7B48
PS3_GAME\USRDIR\Common\res\1_2_2\mob\enderdragon\dragon.png 3E9F5116
PS3_GAME\USRDIR\Common\res\1_2_2\mob\enderdragon\ender.png CD0B501C
PS3_GAME\USRDIR\Common\res\1_2_2\mob\enderdragon\ender_eyes.png 346F2D60
PS3_GAME\USRDIR\Common\res\1_2_2\mob\enderdragon\shuffle.png A914EC0C
PS3_GAME\USRDIR\Common\res\1_2_2\mob\villager\butcher.png E32BCEE4
PS3_GAME\USRDIR\Common\res\1_2_2\mob\villager\farmer.png E9CBA2A2
PS3_GAME\USRDIR\Common\res\1_2_2\mob\villager\librarian.png 8AAA8FB0
PS3_GAME\USRDIR\Common\res\1_2_2\mob\villager\priest.png 5EC81CED
PS3_GAME\USRDIR\Common\res\1_2_2\mob\villager\smith.png 4A01EBA8
PS3_GAME\USRDIR\Common\res\1_2_2\mob\villager\villager.png 633E3281
PS3_GAME\USRDIR\Common\res\1_2_2\terrain\moon.png 6722C3B1
PS3_GAME\USRDIR\Common\res\1_2_2\terrain\moon_phases.png E7FA0D5F
PS3_GAME\USRDIR\Common\res\1_2_2\terrain\sun.png D1FF4020
PS3_GAME\USRDIR\Common\res\TitleUpdate\tutorialDiff 07DE8348
PS3_GAME\USRDIR\Common\res\TitleUpdate\GameRules\Tutorial.pck A6802388
PS3_GAME\USRDIR\Common\res\TitleUpdate\res\colours.col 36E27F56
PS3_GAME\USRDIR\Common\res\TitleUpdate\res\items.png 4BF598BA
PS3_GAME\USRDIR\Common\res\TitleUpdate\res\particles.png EA151F96
PS3_GAME\USRDIR\Common\res\TitleUpdate\res\terrain.png 30FFFFB4
PS3_GAME\USRDIR\Common\res\TitleUpdate\res\terrainMipMapLevel2.png D9011B95
PS3_GAME\USRDIR\Common\res\TitleUpdate\res\terrainMipMapLevel3.png 1D8AD93A
PS3_GAME\USRDIR\Common\res\TitleUpdate\res\armor\cloth_1.png 50FAE9A5
PS3_GAME\USRDIR\Common\res\TitleUpdate\res\armor\cloth_1_b.png E7016547
PS3_GAME\USRDIR\Common\res\TitleUpdate\res\armor\cloth_2.png EBBCE9C4
PS3_GAME\USRDIR\Common\res\TitleUpdate\res\armor\cloth_2_b.png 8393463D
PS3_GAME\USRDIR\Common\res\TitleUpdate\res\armor\power.png F18ECD39
PS3_GAME\USRDIR\Common\res\TitleUpdate\res\art\kz.png AC488023
PS3_GAME\USRDIR\Common\res\TitleUpdate\res\font\Mojangles_11.png 19AD7737
PS3_GAME\USRDIR\Common\res\TitleUpdate\res\font\Mojangles_7.png DF13A82F
PS3_GAME\USRDIR\Common\res\TitleUpdate\res\item\book.png 9904F547
PS3_GAME\USRDIR\Common\res\TitleUpdate\res\item\enderchest.png 18150F86
PS3_GAME\USRDIR\Common\res\TitleUpdate\res\misc\explosion.png 1F08360C
PS3_GAME\USRDIR\Common\res\TitleUpdate\res\misc\footprint.png 038B11F1
PS3_GAME\USRDIR\Common\res\TitleUpdate\res\misc\glint.png 64FDA535
PS3_GAME\USRDIR\Common\res\TitleUpdate\res\misc\mapicons.png 16C5BA38
PS3_GAME\USRDIR\Common\res\TitleUpdate\res\misc\particlefield.png DA331E9B
PS3_GAME\USRDIR\Common\res\TitleUpdate\res\misc\tunnel.png 93B3776F
PS3_GAME\USRDIR\Common\res\TitleUpdate\res\mob\enderman_eyes.png 885725CA
PS3_GAME\USRDIR\Common\res\TitleUpdate\res\mob\redcow.png 7CAF7739
PS3_GAME\USRDIR\Common\res\TitleUpdate\res\mob\skeleton_wither.png 54451A88
PS3_GAME\USRDIR\Common\res\TitleUpdate\res\mob\snowman.png AD43CB53
PS3_GAME\USRDIR\Common\res\TitleUpdate\res\mob\wolf_collar.png 8EE40C46
PS3_GAME\USRDIR\Common\res\TitleUpdate\res\mob\wolf_tame.png 4D04D39D
PS3_GAME\USRDIR\Common\res\TitleUpdate\res\mob\zombie.png FD3CBD6F
PS3_GAME\USRDIR\Common\res\TitleUpdate\res\mob\zombie_villager.png E885B938
PS3_GAME\USRDIR\Common\res\TitleUpdate\res\mob\enderdragon\beam.png 10217676
PS3_GAME\USRDIR\Common\res\TitleUpdate\res\mob\enderdragon\ender.png 495F28AD
PS3_GAME\USRDIR\Common\res\TitleUpdate\res\mob\enderdragon\ender_eyes.png 675D6DD9
PS3_GAME\USRDIR\Common\res\TitleUpdate\res\mob\villager\butcher.png 146C33D8
PS3_GAME\USRDIR\Common\res\TitleUpdate\res\mob\villager\farmer.png A1EC6526
PS3_GAME\USRDIR\Common\res\TitleUpdate\res\mob\villager\librarian.png BB630446
PS3_GAME\USRDIR\Common\res\TitleUpdate\res\mob\villager\priest.png 2F6D772D
PS3_GAME\USRDIR\Common\res\TitleUpdate\res\mob\villager\smith.png 0B26C05A
PS3_GAME\USRDIR\Common\res\TitleUpdate\res\mob\villager\villager.png DD46BB94
PS3_GAME\USRDIR\Common\res\TitleUpdate\res\textures\blocks\fire_0.png 97F1AD2E
PS3_GAME\USRDIR\Common\res\TitleUpdate\res\textures\blocks\fire_0.txt 277A49B1
PS3_GAME\USRDIR\Common\res\TitleUpdate\res\textures\blocks\fire_1.png 22AF2879
PS3_GAME\USRDIR\Common\res\TitleUpdate\res\textures\blocks\fire_1.txt E96CCF45
PS3_GAME\USRDIR\Common\res\TitleUpdate\res\textures\blocks\lava.png CD7679BB
PS3_GAME\USRDIR\Common\res\TitleUpdate\res\textures\blocks\lava.txt 98FB72EE
PS3_GAME\USRDIR\Common\res\TitleUpdate\res\textures\blocks\lava_flow.png D5DDAA4A
PS3_GAME\USRDIR\Common\res\TitleUpdate\res\textures\blocks\lava_flow.txt 459B4141
PS3_GAME\USRDIR\Common\res\TitleUpdate\res\textures\blocks\portal.png 951BD338
PS3_GAME\USRDIR\Common\res\TitleUpdate\res\textures\blocks\portal.txt E96CCF45
PS3_GAME\USRDIR\Common\res\TitleUpdate\res\textures\blocks\water.png B599BA33
PS3_GAME\USRDIR\Common\res\TitleUpdate\res\textures\blocks\water.txt B0DBB880
PS3_GAME\USRDIR\Common\res\TitleUpdate\res\textures\blocks\water_flow.png 329FFB54
PS3_GAME\USRDIR\Common\res\TitleUpdate\res\textures\blocks\water_flow.txt E96CCF45
PS3_GAME\USRDIR\Common\res\TitleUpdate\res\textures\items\clock.png DFDC0AE7
PS3_GAME\USRDIR\Common\res\TitleUpdate\res\textures\items\clock.txt E96CCF45
PS3_GAME\USRDIR\Common\res\TitleUpdate\res\textures\items\compass.png D9DE0C42
PS3_GAME\USRDIR\Common\res\TitleUpdate\res\textures\items\compass.txt E96CCF45
PS3_GAME\USRDIR\Common\res\achievement\bg.png A3AA7039
PS3_GAME\USRDIR\Common\res\achievement\icons.png 46134910
PS3_GAME\USRDIR\Common\res\armor\chain_1.png 98551179
PS3_GAME\USRDIR\Common\res\armor\chain_2.png D27DF6E7
PS3_GAME\USRDIR\Common\res\armor\cloth_1.png AB3306D9
PS3_GAME\USRDIR\Common\res\armor\cloth_2.png E560FD10
PS3_GAME\USRDIR\Common\res\armor\diamond_1.png 0313AEB4
PS3_GAME\USRDIR\Common\res\armor\diamond_2.png 566DF1DA
PS3_GAME\USRDIR\Common\res\armor\gold_1.png E4811C8C
PS3_GAME\USRDIR\Common\res\armor\gold_2.png 3F85A327
PS3_GAME\USRDIR\Common\res\armor\iron_1.png 0DED88AC
PS3_GAME\USRDIR\Common\res\armor\iron_2.png 3EAE0ADE
PS3_GAME\USRDIR\Common\res\armor\power.png F18ECD39
PS3_GAME\USRDIR\Common\res\art\kz.png B96D9B29
PS3_GAME\USRDIR\Common\res\environment\clouds.png 17D31A1B
PS3_GAME\USRDIR\Common\res\environment\rain.png BE2DA7C6
PS3_GAME\USRDIR\Common\res\environment\snow.png B59E9841
PS3_GAME\USRDIR\Common\res\font\default.png E723E088
PS3_GAME\USRDIR\Common\res\font\Mojangles_11.png F0F1DF8F
PS3_GAME\USRDIR\Common\res\font\Mojangles_7.png 77E32356
PS3_GAME\USRDIR\Common\res\gui\background.png 3935ABCF
PS3_GAME\USRDIR\Common\res\gui\container.png B159E8A1
PS3_GAME\USRDIR\Common\res\gui\crafting.png 321C5410
PS3_GAME\USRDIR\Common\res\gui\furnace.png 2EAD9DE1
PS3_GAME\USRDIR\Common\res\gui\gui.png ACBEA6B9
PS3_GAME\USRDIR\Common\res\gui\icons.png 339F3DE5
PS3_GAME\USRDIR\Common\res\gui\inventory.png 10D75239
PS3_GAME\USRDIR\Common\res\gui\items.png CD9BFACA
PS3_GAME\USRDIR\Common\res\gui\logo.png F52A2822
PS3_GAME\USRDIR\Common\res\gui\particles.png E0B9D0BF
PS3_GAME\USRDIR\Common\res\gui\slot.png A2FEC1CC
PS3_GAME\USRDIR\Common\res\gui\trap.png 6443CB39
PS3_GAME\USRDIR\Common\res\gui\unknown_pack.png A36DB965
PS3_GAME\USRDIR\Common\res\item\arrows.png 77DEFE50
PS3_GAME\USRDIR\Common\res\item\boat.png 519215DA
PS3_GAME\USRDIR\Common\res\item\cart.png 33DF18BC
PS3_GAME\USRDIR\Common\res\item\door.png 5CF8128D
PS3_GAME\USRDIR\Common\res\item\sign.png 979C0F4D
PS3_GAME\USRDIR\Common\res\misc\dial.png 4AB6FC2D
PS3_GAME\USRDIR\Common\res\misc\foliagecolor.png 063E03DD
PS3_GAME\USRDIR\Common\res\misc\footprint.png 766E87D3
PS3_GAME\USRDIR\Common\res\misc\grasscolor.png A3698A73
PS3_GAME\USRDIR\Common\res\misc\mapbg.png 4E3A8823
PS3_GAME\USRDIR\Common\res\misc\mapicons.png 1C43BC41
PS3_GAME\USRDIR\Common\res\misc\pumpkinblur.png 71DD2F56
PS3_GAME\USRDIR\Common\res\misc\shadow.png B4CFA661
PS3_GAME\USRDIR\Common\res\misc\vignette.png 3B1BD1FE
PS3_GAME\USRDIR\Common\res\misc\water.png 51F80181
PS3_GAME\USRDIR\Common\res\misc\watercolor.png ED1A8962
PS3_GAME\USRDIR\Common\res\mob\char.png D413391E
PS3_GAME\USRDIR\Common\res\mob\char1.png F00F32BA
PS3_GAME\USRDIR\Common\res\mob\char2.png BF05A5C1
PS3_GAME\USRDIR\Common\res\mob\char3.png 762658E4
PS3_GAME\USRDIR\Common\res\mob\char4.png 4F5366E1
PS3_GAME\USRDIR\Common\res\mob\char5.png 814B362C
PS3_GAME\USRDIR\Common\res\mob\char6.png 76554195
PS3_GAME\USRDIR\Common\res\mob\char7.png 73C724BB
PS3_GAME\USRDIR\Common\res\mob\chicken.png B1520BEF
PS3_GAME\USRDIR\Common\res\mob\cow.png E2751F83
PS3_GAME\USRDIR\Common\res\mob\creeper.png C43EF4C7
PS3_GAME\USRDIR\Common\res\mob\ghast.png 987C4E4C
PS3_GAME\USRDIR\Common\res\mob\ghast_fire.png A35C999C
PS3_GAME\USRDIR\Common\res\mob\pig.png 402663BF
PS3_GAME\USRDIR\Common\res\mob\pigman.png 50143A85
PS3_GAME\USRDIR\Common\res\mob\pigzombie.png CC98A297
PS3_GAME\USRDIR\Common\res\mob\saddle.png D90F1367
PS3_GAME\USRDIR\Common\res\mob\sheep.png 29CD6D81
PS3_GAME\USRDIR\Common\res\mob\sheep_fur.png 4A5064B6
PS3_GAME\USRDIR\Common\res\mob\skeleton.png EADAC7FD
PS3_GAME\USRDIR\Common\res\mob\slime.png A27DA092
PS3_GAME\USRDIR\Common\res\mob\spider.png 5963D360
PS3_GAME\USRDIR\Common\res\mob\spider_eyes.png 7A366D75
PS3_GAME\USRDIR\Common\res\mob\squid.png 9828FC11
PS3_GAME\USRDIR\Common\res\mob\wolf.png 21499859
PS3_GAME\USRDIR\Common\res\mob\wolf_angry.png 156D783E
PS3_GAME\USRDIR\Common\res\mob\wolf_tame.png F9700274
PS3_GAME\USRDIR\Common\res\mob\zombie.png 67EFD9C4
PS3_GAME\USRDIR\Common\res\terrain\moon.png 6722C3B1
PS3_GAME\USRDIR\Common\res\terrain\sun.png B5C7F054
PS3_GAME\USRDIR\DLC\Battle & Beasts\BattleAndBeasts.pck 171E1672
PS3_GAME\USRDIR\DLC\City Texture Pack\TexturePack.pck E86B6920
PS3_GAME\USRDIR\DLC\City Texture Pack\Data\media.arc E70D4245
PS3_GAME\USRDIR\DLC\City Texture Pack\Data\x32Data.pck 3297C4E1
PS3_GAME\USRDIR\DLC\Festive Skin Pack\SkinsFestive.pck 22CB8342
PS3_GAME\USRDIR\DLC\Plastic Texture Pack\TexturePack.pck 9501BB8C
PS3_GAME\USRDIR\DLC\Plastic Texture Pack\Data\media.arc C3040075
PS3_GAME\USRDIR\DLC\Plastic Texture Pack\Data\x16Data.pck 1CDCF857
PS3_GAME\USRDIR\DLC\Skin Pack 1\Skins1_Sony.pck E7C4C19E
PS3_GAME\USRDIR\PS3\PS3ProductCodes.bin 7F4D55CC
PS3_GAME\USRDIR\PS3\Sound\Minecraft.msscmp 36384AFB
PS3_GAME\USRDIR\music\cds\11.binka 60710803
PS3_GAME\USRDIR\music\cds\13.binka E637D3B3
PS3_GAME\USRDIR\music\cds\blocks.binka C74949CB
PS3_GAME\USRDIR\music\cds\cat.binka 2B5BAC99
PS3_GAME\USRDIR\music\cds\chirp.binka 4CE7E4DA
PS3_GAME\USRDIR\music\cds\far.binka C1785D02
PS3_GAME\USRDIR\music\cds\mall.binka DFB0D353
PS3_GAME\USRDIR\music\cds\mellohi.binka 49870A92
PS3_GAME\USRDIR\music\cds\stal.binka 33A19C97
PS3_GAME\USRDIR\music\cds\strad.binka ADC985B4
PS3_GAME\USRDIR\music\cds\ward.binka E3C87026
PS3_GAME\USRDIR\music\cds\where_are_we_now.binka 9DC2221A
PS3_GAME\USRDIR\music\music\calm1.binka E7E919DB
PS3_GAME\USRDIR\music\music\calm2.binka 88FE5E90
PS3_GAME\USRDIR\music\music\calm3.binka 21BD7501
PS3_GAME\USRDIR\music\music\hal1.binka 2B8E2BDE
PS3_GAME\USRDIR\music\music\hal2.binka 121EB1CF
PS3_GAME\USRDIR\music\music\hal3.binka E1DC06E3
PS3_GAME\USRDIR\music\music\hal4.binka D99E922C
PS3_GAME\USRDIR\music\music\nether1.binka B9A1E324
PS3_GAME\USRDIR\music\music\nether2.binka 1B5091AB
PS3_GAME\USRDIR\music\music\nether3.binka A2A66875
PS3_GAME\USRDIR\music\music\nether4.binka 1361AEE7
PS3_GAME\USRDIR\music\music\nuance1.binka FF52867A
PS3_GAME\USRDIR\music\music\nuance2.binka 6F426454
PS3_GAME\USRDIR\music\music\piano1.binka 372B14E0
PS3_GAME\USRDIR\music\music\piano2.binka 79CA781D
PS3_GAME\USRDIR\music\music\piano3.binka B0113BEA
PS3_GAME\USRDIR\music\music\the_end_dragon_alive.binka 21CFAB35
PS3_GAME\USRDIR\music\music\the_end_end.binka 0486F2C7
PS3_UPDATE\PS3UPDAT.PUP 88623F05</pre>

Credits:

Utilizes 7-Zip 18.05 (x64) : Copyright (c) 1999-2018 Igor Pavlov : 2018-04-30