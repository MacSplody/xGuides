## Manual Cleaning Guides

### Wild Edits

1. [Teleport - City Spells](#-teleport---city-spells-)
2. [Teleport - Faction Spells](#-teleport---faction-spells-)
3. [Teleport - Towns and Villages](#-teleport---towns-and-villages-)
4. [Moon & Star](#-moon-and-star-)
5. [Distinct Interiors](#-distinct-interiors-)

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
- Right click the empty field of the `XCCM` subrecord and from the context menu select `Add`.
  ![image](pics/TFS-000AD5A1-ADD.png)
- You should now see a `Null` formid value in the field of the `XCCM` subrecord.  
  ![image](pics/TFS-000AD5A1-Null.png)
- Right click the NULL value and select edit from the context menu.
  ![image](pics/TFS-000AD5A1-EditSelect.png)
- Replace the `Null` value with `0002A72D` and select ok.
  ![image](pics/TFS-000AD5A1-Edit.png)
- You should now see the value `WeatherPineForest` in the field of the `XCCM` subrecord of Faction Teleport Spells.
  ![image](pics/TFS-000AD5A1-FIN.png)
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
- Right click and select none.
- Select `Heartfires.esm` and `MoonAndStar_MAS.esp`.
- Add `Heartfires.esm` as a master to `MoonAndStar_MAS.esp`.

  ![image](pics/MAS-addmaster.png)
  ![image](pics/MAS-addmasters-selection.png)

- Open record `000166A9`

  ![image](pics/MAS-000166A9-before-drag-navm.png)

- Drag & Drop these values from `Heartfires.esm` to `MoonAndStar_MAS.esp`.
    
    - `Navigation Mesh`

  ![image](pics/MAS-000166A9-before-drag-navm.png)

  ![image](pics/MAS-000166A9-after-drop-navm.png)
    
    - `Teleport Marker Triangle`

  ![image](pics/MAS-000166A9-before-drag-TMT.png)

  ![image](pics/MAS-000166A9-after-drop-TMT.png)

The Wild edits are now corrected, you can save the changes to the cleaned plugin with `ctrl+s` or when prompted before exiting SSEEdit.

---

### [ Distinct Interiors ](https://www.nexusmods.com/skyrimspecialedition/mods/6130/)

`Distinct Interiors.esp`  
or  
`Distinct Interiors - Player Homes.esp`

#### Edit the following record(s) with SSEEdit
- Remove the deleted record `000CB4F3` from `Distinct Interiors.esp`
  ![image](pics/DIAIO-000CB4F3.png)

The Wild edits are now corrected, you can save the changes to the cleaned plugin with `ctrl+s` or when prompted before exiting SSEEdit.
