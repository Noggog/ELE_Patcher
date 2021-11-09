# Mod support details
For the curious & for my own reference.

Lists what the patcher changes for each supported mod, and what, if anything, is different from the patch that part of the patcher is based on.  
Said differences from the base patch are marked with **bold** in general, and in the dropdown lists with
```diff 
- Red for removed
+ Green for added
! Orange for special cases
```

## Based on patches available from [ELE's optional downloads](https://www.nexusmods.com/skyrimspecialedition/mods/1377?tab=files)
With updates here & there as said patches are 2 years old. Changes marked with *.

[//]: # (comment <details><summary>Expand to see the changes</summary>)

- [Beyond Skyrim - Bruma SE](https://www.nexusmods.com/skyrimspecialedition/mods/10917) (1.4.2)
  - Cell changes
    - Lighting templates, inherits flags & image spaces
      - Some use a custom `ELE_Patcher_1ELE_DungeonAyleid_IS` image space
    - **Removed & added changes for some cells**<details><summary>**Expand for full list**</summary>
      ```diff
      - CYRAleswellCrextusResidence
      - CYRAleswellFalegusResidence
      - CYRAleswellInn
      - CYRAleswellMathiasEndieriHouse
      - CYRAleswellUmogDarSeelHouse
      - CYRCloudTopLookout
      - CYRCrumblingMine
      - CYRDirichKeepFarmhouse
      - CYRDzonotCave
      + CYRForesterOutpostForestMountainInterior01
      - CYRFortCaractacus01
      - CYRFortColdcorn01
      - CYRFortColdcorn02
      - CYRFortHomestead
      - CYRFortRayles01
      - CYRFrostCragSpireVault
      - CyrGarlasAgea
      - CyrGarlasTure
      - CYRGnollPass01
      - CYRLakesideRetreat
      - CYRLighthouseGoldCoast
      - CYRMountainWatchAvringErvigHouse
      - CYRMountainWatchAubertHouse
      - CYRMountainWatchBunkhouse
      - CYRMountainWatchZurikkiHouse
      - CYRNorthfringeSanctum03
      - CYRNorthfringeSanctum04
      - CYRNorthfringeSanctum05
      - CYROutlawEndreCave
      - CYRPellsGateInterior01BlacielAnHouse
      - CYRSedor
      - CyrSidewaysCave01
      - CyrSidewaysCave02
      - CyrSidewaysCave03
      - CYRWatersEdgeInterior06
      - CYRWellappBanditMine
      - CYRWeyeBastienAdrardHouse
      - CYRWeyeDominitianFarm
      - CYRWeyeDurashGraAgumHouse
      - CYRWeyeGeneralStore
      - CYRWeyeGrennHouse
      - CYRWeyeMessalaFarm
      - CYRWeyeWarehouseAux
      ```
      </details>
  - Light changes
    - Colors
      - `CYRAyleidWhite` lights get their own custom color
    - **Added changes for `CYRAyleidWhiteLightShadow02`**
- [Cutting Room Floor - SSE](https://www.nexusmods.com/skyrimspecialedition/mods/276) (3.1.9)
  - Cell changes
    - Lighting templates, **inherits flags** & image spaces
    - **Added changes for `CRFStonehillsGesturHouse`**
- [Darkend](https://www.nexusmods.com/skyrimspecialedition/mods/10423) (1.4)
  - Cell changes
    - Image spaces
  - Light changes
    - Color, flags & fade value for `XJKTorch01Shadow256`
- [Falskaar](https://www.nexusmods.com/skyrimspecialedition/mods/2057) (2.2)
  - Cell changes
    - Lighting templates, inherits flags & image spaces
    - **Removed changes for some cells**<details><summary>**Expand for full list**</summary>
      ```diff
      - FSIceFort
      - FSStargazerGrove
      ```
      </details>
- [Helgen Reborn](https://www.nexusmods.com/skyrimspecialedition/mods/5673) (V106.SSE)
  - Cell changes
    - Lighting templates, inherits flags & image spaces
    - **Removed changes for some cells**<details><summary>**Expand for full list**</summary>
      ```diff
      - aaaBalokAerandilShip
      - aaaBalokCrypt01
      - aaaBalokDoorRoom
      ```
      </details>
  - **Light changes**
    - **Color for `BalokBrazierLightsCavern`**
- [Lanterns of Skyrim](https://www.nexusmods.com/skyrimspecialedition/mods/2429) (any version)
  - Light changes
    - Color & fade value for `mannyLanternsOfSkyrimAllInOne`
- [Legacy of the Dragonborn SSE](https://www.nexusmods.com/skyrimspecialedition/mods/11802) (5.5.2, 4.1.1 support included)
  - **v5 detection**
    - Brighter lighting templates & image spaces for v5 museum cells
  - Cell changes
    - Minor lighting changes, lighting templates, inherits flags & image spaces
    - **Modified & added changes for some cells, orange ones subject to v5 detection**<details><summary>**Expand for full list**</summary>
      ```diff
      ! DBMDGAetheriumRoom
      ! DBMDGArmory
      ! DBMDGArmoryEast
      ! DBMDGArmoryLower
      ! DBMDGArmoryWest (2 FormIDs)
      ! DBMDGArmourySouth
      ! DBMDGBookStacks
      ! DBMDGCultureandArt
      ! DBMDGDaedricHall
      ! DBMDGDragonbornHall
      ! DBMDGEastExhibitHalls / DBMDGHallofLostEmpires
      ! DBMDGHallofHeroes
      ! DBMDGHallofHeroesHeist
      ! DBMDGHallofHeroesHaunted
      ! DBMDGHallofLegends
      ! DBMDGHallofOddities
      ! DBMDGHallofSecrets
      ! DBMDGHallofSecretsBare
      ! DBMDGNaturalScience
      ! DBMDGNaturalScienceHaunted (2 FormIDs)
      ! DBMDGLibrary
      ! DBMDGSafehouse
      ! DBMDGUpperGallery
      ! DBMDGWineCellar
      ! DBMGuildhouse
      ! DBMDGStoreroom
      + DBMRainsShelter
      + DLC2MoesringPass02DBM
      ```
      </details>
  - Image space changes
    - Cinematic for `DBM_HauntedMuseumIMG`
  - Light changes
    - Color for `DBM_Torch` and `DBM_TorchREPLICA`
- [Medieval Lanterns of Skyrim](https://www.nexusmods.com/skyrimspecialedition/mods/27622) (any version)
  - Light changes
    - Color for `MLOS_candlelight_01`
- [Ravengate](https://www.nexusmods.com/skyrimspecialedition/mods/12617) (0.06BTASSE)
  - Cell changes
    - Lighting templates, **inherits flags** & image spaces
  - **Light changes**
    - Color
    - **Added changes for lights**<details><summary>**Expand for full list**</summary>
      ```diff
      + RVH_Light_BurnItDownx
      + RVH_Light_DeathFire
      + RVH_Light_DefaultCandleLight01NSDesat_Bright
      + RVH_Light_DefaultCandleLight01NS_Bright
      + RVH_Light_DefaultCandleLight01NS_Loraliah
      + RVH_Light_DefaultCandleLight01NS_Saturated
      + RVH_Light_DefaultCandleLight01NS_Saturated_Hemi
      + RVH_Light_DefaultTorch01NS_Bright
      + RVH_Light_LightCampFire01_Arena
      + RVH_Light_LightCampFire01_Shadows
      + RVH_Light_Oblivion_Fire
      ```
      </details>

[//]: # (</details>)

[//]: # (comment template)