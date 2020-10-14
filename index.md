## Manual Cleaning Guides

### Wild Edits

1. [Teleport - City Spells](#-teleport---city-spells-)
2. [Teleport - Faction Spells](#-teleport---faction-spells-)
3. [Teleport - Towns and Villages](#-teleport---towns-and-villages-)
4. [Moon & Star](#-moon-and-star-)
5. [Undeath: Remastered SSE](#-undeath-remastered-)

### Deleted navmeshes
1. [Distinct Interiors](#-distinct-interiors-)

### Unresolved Reference
##### USSEP Aventus Aretino Package
1. [RS Children Overhaul](#-rs-children-overhaul-)
2. [Axe's RS Children](#-axes-rs-children-)
3. [Killable Children](#-killable-children-)
4. [Simple Children](#-simple-children-)
5. [TK Children](#-tk-children-)
6. [Children](#-children-)

---

### [ Teleport - City Spells ](https://www.nexusmods.com/skyrimspecialedition/mods/7015/)

`TheWulfPanda - City Teleport Spells.esp`  
or  
`TheWulfPanda - City Teleport Spells Less Magicka Increase Cast Time.esp`

#### Edit the following record(s) with SSEEdit
1. Remove record `0000939D`![image](pics/TCS-0000939D.png)
2. Remove record `00037EE9`![image](pics/TCS-00037EE9.png)
3. Remove record `0001A27F`![image](pics/TCS-0001A27F.png)
4. Remove record `00020EE7`![image](pics/TCS-00020EE7.png)
5. Remove record `00042249`![image](pics/TCS-00042249.png)

The Wild edits are now corrected, you can save the changes to the cleaned plugin with `ctrl+s` or when prompted before exiting SSEEdit.

---

### [ Teleport - Faction Spells ](https://www.nexusmods.com/skyrimspecialedition/mods/6991/)

`TheWulfPanda - Faction Teleport Spells.esp`  
or  
`TheWulfPanda - Faction Teleport Spells Less Magicka Increased Cast Time.esp`

#### Edit the following record(s) with SSEEdit

1. Remove the Worldspace record.![image](pics/TFS-WRLD.png)
2. Remove the record `02010521`.![image](pics/TFS-02010521.png)
3. Remove the record `02007320`.![image](pics/TFS-02007320.png)
4. Remove the record `000CA72C`.![image](pics/TFS-000CA72C.png)
5. Remove the record `000B3434`.![image](pics/TFS-000B3434.png)
6. Remove the record `000C0291`.![image](pics/TFS-000C0291.png)
7. Open cell record `000AD5A1`.![image](pics/TFS-000AD5A1-Rec.png)
  - Right click the empty field of the `XCCM` subrecord and from the context menu select `Add`.![image](pics/TFS-000AD5A1-ADD.png)
  - You should now see a `Null` formid value in the field of the `XCCM` subrecord.![image](pics/TFS-000AD5A1-Null.png)
  - Right click the NULL value and select edit from the context menu.![image](pics/TFS-000AD5A1-EditSelect.png)
  - Replace the `Null` value with `0002A72D` and select ok.![image](pics/TFS-000AD5A1-Edit.png)
  - You should now see the value `WeatherPineForest` in the field of the `XCCM` subrecord of Faction Teleport Spells.![image](pics/TFS-000AD5A1-FIN.png)
8. `00016BCF` Remove `XEZN` subrecord referring to RiftenRatwayZone `[ECZN:0009FBB9]`![image](pics/TFS-00016BCF.png)
- The Wild edits are now corrected, you can save the changes to the cleaned plugin with `ctrl+s` or when prompted before exiting SSEEdit.

---

### [ Teleport - Towns and Villages ](https://www.nexusmods.com/skyrimspecialedition/mods/7267/)

`TheWulfPanda - Teleport Spells Towns and Villages.esp`  
or  
`TheWulfPanda - Teleport Spells Towns and Villages Less Magicka Increase Cast Time.esp`

#### Edit the following record(s) with SSEEdit
- Remove cell record DragonBridgeExterior03 `00009349`
![image](pics/TTW-00009349.png)
- Remove cell record Riverwood `00009732`
![image](pics/TTW-00009732.png)
- Remove cell record IvarsteadExterior02 `000097BF`.
![image](pics/TTW-000097BF.png)
- Remove the value in subrecord `XCWT` of cell record `00009731`.
![image](pics/TTW-00009731.png)

The Wild edits are now corrected, you can save the changes to the cleaned plugin with `ctrl+s` or when prompted before exiting SSEEdit.

---

### [ Moon and Star ](https://www.nexusmods.com/skyrimspecialedition/mods/4301/)

`MoonAndStar_MAS.esp`

#### Edit the following record(s) with SSEEdit
- Open SSEEDIT.
- Right click the module selection window.
- `Select none` from the context menu.![image](pics/MAS-Select-none.png)
- Then select only the `DLC` & `MoonAndStar_MAS.esp`.![image](pics/MAS-Module-Selection.png)
- In the left panel, right click `MoonAndStar_MAS.esp`.
- Select `Add masters` from the context menu.![image](pics/MAS-addmaster.png)
- Tick `Heartfires.esm` and click okay.![image](pics/MAS-addmasters-selection.png)

1. Open record `000166A9` and scroll down to the subrecord `XNDP - Navigation Door Link`.![image](pics/MAS-000166A9-before-drag-navm.png)
2. Drag & Drop the values in subrecord `XNDP - Navigation Door Link` from `Heartfires.esm` into `MoonAndStar_MAS.esp`.![image](pics/MAS-000166A9-before-drag-navm.png)![image](pics/MAS-000166A9-after-drop-TMT.png)
3. Open `cell` record `00009B37` and scroll down to the subrecord `XCWT - Water`.Drag & Drop the value in the `XCWT - Water` subrecord from `Update.esm` into `MoonAndStar_MAS.esp`![image](pics/MAS-00009B37-XCWT.png)![image](pics/MAS-00009B37-XCWT-After.png)

4. The following records also need the `XCWT - Water` subrecord value copied from `Update.esm` into `MoonAndStar_MAS.esp`.
   - `00009B54`, `00009B55`, `00009B56`, `00009B57`, `00009B58`,
   - `00009B75`, `00009B76`, `00009B77`, `00009B78`,
   - `00009B97`, `00009B98`, `00009B99`, `00009B9A`, `00009B9B`,
   - `00009BB8`, `00009BB9`, `00009BBA`, `00009BBB`,

5. `00000D74` Drag and drop the `XCLR - Regions` subrecord from `Dawnguard.esm` on to the corresponding empty subrecord in `MoonAndStar_MAS.esp`.![image](pics/MAS-00000D74-before.png)![image](pics/MAS-00000D74-after.png)

The Wild edits are now corrected, you can save the changes to the cleaned plugin with `ctrl+s` or when prompted before exiting SSEEdit.

---

### [ Undeath Remastered ](https://www.nexusmods.com/skyrimspecialedition/mods/6180/)

`Undeath.esp`

Remove the following records:

   _Armor_

   - `0003B5AB` SkinDragonPriest
   - `000B799A` SkinSkeleton
   - `0010CFE4` ClothesMonkRobesColorBrownHooded
   - `0010CFEA` ClothesMonkRobesColorGreyHooded
   - `0010CFEB` ClothesMonkRobesColorRedHooded
   - `0010CFEC` ClothesMonkRobesColorGreenHooded
   
   ![image](pics/Undeath/Armor-Overview-Before.png)
   ![image](pics/Undeath/Armor-Overview-Remove.png)
   ![image](pics/Undeath/Armor-Overview-Remove-Yes.png)
   ![image](pics/Undeath/Armor-Overview-After.png)

  _Magic Effect_

   - `0001CEAA` SummonFlameAtronach
   - `0001CEAB` SummonFrostAtronach
   - `0001CEAC` SummonStormAtronach
   - `000640B4` SummonFamiliar
   - `0006A154` MGRSummonArnielEffect
   - `0007E5D2` SummonFlameThrall
   - `0007E5D3` SummonFrostThrall
   - `0007E5D4` SummonStormThrall
   - `0007E8E0` ReanimateThrallFFAimed
   - `000A88C8` dunRannveigSummonGhost
   - `000CDECF` SummonFlameThrallPotent
   - `000CDED0` SummonFrostThrallPotent
   - `000CDED1` SummonStormThrallPotent
   - `0010DDED` SummonDremoraLord
   - `0010EE48` SummonFrostAtronachNPC
   - `0010EE49` SummonStormAtronachNPC
   - `0010FC12` SummonDragonPriest
   - `01000840` EnchSummonFlameAtronach
   - `01000841` EnchSummonFrostAtronach
   - `01000842` EnchSummonStormAtronach
   - `01000843` EnchSummonFlameThrall
   - `01000844` EnchSummonFrostThrall
   - `01000845` EnchSummonStormThrall
   - `020045B5` SummonWrathman
   - `020045BB` SummonMistman
   - `020045BC` SummonBoneman
   - `0200C601` DLC01SummonSoulHorseEffect
   - `0200E7D7` DLC1nVampireBloodyGripCloakEffect

   ![image](pics/Undeath/Magic-Overview-01-Before.png)
   ![image](pics/Undeath/Magic-Overview-02-Before.png)
   ![image](pics/Undeath/Magic-Overview-Remove.png)
   ![image](pics/Undeath/Magic-Overview-Remove-Yes.png)
   ![image](pics/Undeath/Magic-Overview-After.png)

  _Non-Player Character (Actor)_

   - `0001E7CA` LvlWarlockNecromancer
   - `0002D1DE` EncSkeleton01Melee1H
   - `0002D1E0` EncSkeleton01Melee2H
   - `0002D1FC` EncSkeleton01Missile
   - `0002D1FD` EncSkeleton01Melee1Hshield
   - `0003B547` EncDraugr01Template
   - `0003BE1E` EncDraugr01TemplateMissile
   - `000524E5` EncSkeleton01AmbushMelee1H
   - `000548FE` EncWarlock01TemplateNecro
   - `0005B752` EncDraugr01Template2H
   - `000C3B1C` TreasCorpseSkeleton
   - `000DA06B` EncSkeleton01AmbushMelee1HShield
   - `02010E9B` DLC1lvlDragonIceLake
   - `02011CD2` AudioTemplateVampireLord
   - `020145A5` DLC1VQ02VampLordLoadDummy
   - `0201A93D` DLC1HarkonCombat
   - `0301E290` AudioTemplateWerebear
   - `0303D588` AudioTemplateRiekling
   - `0303D589` AudioTemplateRieklingQuiet
   
   ![image](pics/Undeath/NPCs-Overview-Before.png)
   ![image](pics/Undeath/NPCs-Overview-Remove.png)
   ![image](pics/Undeath/NPCs-Overview-Remove-Yes.png)
   ![image](pics/Undeath/NPCs-Overview-After.png)

  _Perk_

   - `00106092` doomRitualPerk

   ![image](pics/Undeath/Perk-Overview-Before.png)
   ![image](pics/Undeath/Perk-Overview-Remove.png)
   ![image](pics/Undeath/Perk-Overview-Remove-Yes.png)
   ![image](pics/Undeath/Perk-Overview-After.png)

  _Spell_

   - `000204C4` ConjureFrostAtronach
   - `000204C5` ConjureStormAtronach
   - `000211EF` DetectDead
   - `000640B6` ConjureFamiliar
   - `0007E8DF` DeadThrall
   - `0007E8E4` Blizzard
   - `00096D94` Revenant
   - `0009BCCA` AbDragonPriest
   - `000A1992` IceStormLeftHand
   - `000ABDF3` ConjureFrostAtronachLeftHand
   - `000BB967` ConjureFlameAtronachLeftHand
   - `000BB968` ConjureStormAtronachLeftHand
   - `000C969C` IceSpikeRightHand
   - `000C969E` RaiseZombieLeftHand
   - `000E1529` dunReanimateSelf
   - `000E7329` doomRitualAbility
   - `00100E75` ConjureFamiliarRightHand
   - `00100E76` ConjureFlameAtronachRightHand
   - `00100E77` ConjureFrostAtronachRightHand
   - `00100E78` ConjureStormAtronachRightHand
   - `0010DDEC` ConjureDremoraLord
   - `0010FC16` ConjureDragonPriest
   - `020038B7` DLC1VampiresGrip
   - `020045B3` DLC1ConjureWrathman
   - `020045B8` DLC1ConjureMistman
   - `020045BA` DLC1ConjureBoneman
   - `02016909` DLC1ConjureGargoyleLeftHand
   - `0301CDF6` DLC2ConjureAshSpawn
   - `03029F12` DLC2ConjureBardInstruments
   - `03033C66` DLC2ConjureSeeker
   - `0303D473` DLC2ConjureAshGuardianLeftHand

   ![image](pics/Undeath/Spell-Overview-01-Before.png)
   ![image](pics/Undeath/Spell-Overview-02-Before.png)
   ![image](pics/Undeath/Spell-Overview-Remove.png)
   ![image](pics/Undeath/Spell-Overview-Remove-Yes.png)
   ![image](pics/Undeath/Spell-Overview-After.png)

Edit the following records:

The `XCWT - Water` subrecord value in `Undeath.esp` must be changed to match the value in `Update.esm`.

   - `000092DE`
   - `000092DF` SolitudeSewersSouthExt
   - `000092E0`
   - `00009300`
   - `000094B8`
   - `00009A60` NecroCaravanExt01
   - `00009B98`
   - `00009BB9` NecroArkayShrineExt01
   - `00009BBA`
   
   ![image](pics/Undeath/Filter-Overview-Before.png)

   Right click `Undeath.esp`, and select _Apply Filter (Selected files only)_

   ![image](pics/Undeath/Filter-Overview-Apply.png)

   Apply the checkboxes indicated by the arrows in the following image and then select Filter.

   ![image](pics/Undeath/Filter-Overview-Options.png)

   This will filter to leave only records that are reverting changes.
   ![image](pics/Undeath/Filter-Overview-After.png)

   To copy a sub-record value, you can drag and drop it from one plugin to another in the right panel.
   ![image](pics/Undeath/Waterflow-Overview-Before.png)
   ![image](pics/Undeath/Waterflow-Overview-During.png)
   ![image](pics/Undeath/Waterflow-Overview-After-first.png)

   ![image](pics/Undeath/Waterflow-Overview-All-First.png)

   To remove a sub-record value, right click it in the right panel and select remove.
   ![image](pics/Undeath/Waterflow-Remove-Before.png)
   ![image](pics/Undeath/Waterflow-Remove-During.png)
   ![image](pics/Undeath/Waterflow-Remove-After.png)

   ![image](pics/Undeath/Waterflow-Overview-After-All.png)

The Wild edits are now corrected, you can save the changes to the cleaned plugin with `ctrl+s` or when prompted before exiting SSEEdit.

---

### [ Distinct Interiors ](https://www.nexusmods.com/skyrimspecialedition/mods/6130/)

`Distinct Interiors.esp`  
or  
`Distinct Interiors - Player Homes.esp`

#### Edit the following record(s) with SSEEdit
- Remove the deleted record `000CB4F3` from `Distinct Interiors.esp`
  ![image](pics/DIAIO-000CB4F3.png)

The Deleted navmeshes are now corrected, you can save the changes to the cleaned plugin with `ctrl+s` or when prompted before exiting SSEEdit.

---

### [ RS Children Overhaul ](https://www.nexusmods.com/skyrimspecialedition/mods/2650/)

`RSChildren.esp`

#### Edit the following record(s) with SSEEdit
- Remove the unresolved reference in record `00014132` AventusAretino Packages from `RSChildren.esp`

  ![image](pics/RSC-AA-00.png)

  ![image](pics/RSC-AA-01.png)

  ![image](pics/RSC-AA-02.png)

  ![image](pics/RSC-AA-03.png)

The unresolved reference is now corrected, you can save the changes to the cleaned plugin with `ctrl+s` or when prompted before exiting SSEEdit.

---

### [ Axe's RS Children ](https://www.nexusmods.com/skyrimspecialedition/mods/16044/)

`aAxeRSCtweaks.esp`

#### Edit the following record(s) with SSEEdit
- Remove the unresolved reference in record `00014132` AventusAretino Packages from `aAxeRSCtweaks.esp`

  ![image](pics/AXERSC-AA-00.png)

  ![image](pics/AXERSC-AA-01.png)

  ![image](pics/AXERSC-AA-02.png)

  ![image](pics/AXERSC-AA-03.png)

The unresolved reference is now corrected, you can save the changes to the cleaned plugin with `ctrl+s` or when prompted before exiting SSEEdit.

---

### [ Killable Children ](https://www.nexusmods.com/skyrimspecialedition/mods/1108/)

`Killable Children.esp`

#### Edit the following record(s) with SSEEdit
- Remove the unresolved reference in record `00014132` AventusAretino Packages from `Killable Children.esp`

  ![image](pics/KC-AA-00.png)

  ![image](pics/KC-AA-01.png)

  ![image](pics/KC-AA-02.png)

  ![image](pics/KC-AA-03.png)

The unresolved reference is now corrected, you can save the changes to the cleaned plugin with `ctrl+s` or when prompted before exiting SSEEdit.

---

### [ Simple Children ](https://www.nexusmods.com/skyrimspecialedition/mods/22789/)

`FacegenForKids.esp`

#### Edit the following record(s) with SSEEdit
- Remove the unresolved reference in record `00014132` AventusAretino Packages from `FacegenForKids.esp`

  ![image](pics/SCFFK-00.png)

  ![image](pics/SCFFK-01.png)

  ![image](pics/SCFFK-02.png)

  ![image](pics/SCFFK-03.png)

The unresolved reference is now corrected, you can save the changes to the cleaned plugin with `ctrl+s` or when prompted before exiting SSEEdit.

---

### [ TK Children ](https://www.nexusmods.com/skyrimspecialedition/mods/5916/)

`TKChildren.esp`

#### Edit the following record(s) with SSEEdit
- Remove the unresolved reference in record `00014132` AventusAretino Packages from `TKChildren.esp`

  ![image](pics/TKC-00.png)

  ![image](pics/TKC-01.png)

  ![image](pics/TKC-02.png)

  ![image](pics/TKC-03.png)

The unresolved reference is now corrected, you can save the changes to the cleaned plugin with `ctrl+s` or when prompted before exiting SSEEdit.

---

### [ Children ](https://www.nexusmods.com/skyrimspecialedition/mods/2822/)

`Children.esp`

#### Edit the following record(s) with SSEEdit
- Remove the unresolved reference in record `00014132` AventusAretino Packages from `Children.esp`

  ![image](pics/CHI-00.png)

  ![image](pics/CHI-01.png)

  ![image](pics/CHI-02.png)

  ![image](pics/CHI-03.png)

The unresolved reference is now corrected, you can save the changes to the cleaned plugin with `ctrl+s` or when prompted before exiting SSEEdit.