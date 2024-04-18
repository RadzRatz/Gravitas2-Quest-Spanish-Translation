# Changelog

# 📦 0.2.7-a

## 📰 General changes and notes

Summary of changes here!

<details open>
<summary>Github Commits :octocat:</summary>
<blockquote>

- fix recipes being voided in EBF and other machines
- how tf does this even happen lol
- fix bucket dupe
- fix chalk recipe conflict
- add treated wood slabs
- fix alumin(i)um fences
- restrict to TFC worlds only
- Add Create Igneous Alloy to GTCE Alloy Smelter
- Add Create Igneous Alloy to GTCE Alloy Smelter
- add macerator recipes for loose stone -> dusts
- reduce processing times for Gael
- resolves #208
- resolves #209
- remove conflicting recipe
- add tfc thermal deposits config</blockquote>

</details>

---

## 🛠️ Mods

<details open>
<summary>Added (5)</summary>

- Create: More Drill Heads (2.0.3-1.20.1)
- Falling Trees (0.10)
- PandaLib (0.1)
- Player Animator (1.0.2-rc1+1.20)
- Sitting+ (1.0.1)

</details>

<details>
<summary>Updated (28)</summary>

- Advanced TFC Tech Unofficial (2.1) -> (2.2)
- Applied Energistics 2 (15.0.21) -> (15.0.23)
- AllTheTweaks (2.2.0) -> (2.2.2)
- AlmostUnified (1.20.1-0.8.1) -> (1.20.1-0.9.2)
- Apotheosis (7.3.1) -> (7.3.3)
- Athena (3.1.1) -> (3.1.2)
- Apothic Attributes (1.3.0) -> (1.3.3)
- Create: Connected (0.7.2-mc1.20.1) -> (0.7.4-mc1.20.1)
- CreativeCore (2.11.24) -> (2.11.25)
- Cupboard utilities (1.20.1-2.5) -> (1.20.1-2.6)
- Curios API (5.7.0+1.20.1) -> (5.7.2+1.20.1)
- Ender IO (6.0.24-alpha) -> (6.0.25-alpha)
- ExtendedAE (1.20-1.0.13-forge) -> (1.20-1.0.16-forge)
- FramedBlocks (9.2.0) -> (9.2.1)
- FTB Chunks (2001.2.5) -> (2001.2.6)
- FTB Quests (2001.3.3) -> (2001.3.4)
- FTB Teams (2001.1.4) -> (2001.2.0)
- Gravitas² Core Mod (1.0.33) -> (1.0.34)
- Lootr (0.7.31.77) -> (0.7.32.79)
- Macaw's All-In-One for TFC (0.2.14-1.20.1) -> (0.2.30-1.20.1)
- Moonlight Library (1.20-2.10.10) -> (1.20-2.11.7)
- MoreJS (0.6.0) -> (0.7.0)
- Puzzles Lib (8.1.17) -> (8.1.18)
- Stargate Journey (0.6.21) -> (0.6.22)
- SparseStructuresReforged (1.20.1-1.0.0) -> (1.20.1-0.0.1)
- TFC Thermal Deposits (1.3.8) -> (1.3.9a)
- Corail Tombstone (8.6.3) -> (8.6.4)
- Create: Vintage Improvements (1.20.1-0.1.2.0) -> (1.20.1-0.1.3.2)

</details>

## 🍳 Recipes

<details>
<summary>Added (166)</summary>
<blockquote>

<details>
<summary>allthetweaks/greg_star_block</summary>

```diff
+{
+  type: "minecraft:crafting_shaped"
+  category: "misc"
+  group: "allthetweaks"
+  key: {
+    a: {
+      tag: "allthetweaks:greg_star"
+    }
+  }
+  pattern: [
+    "aaa"
+    "aaa"
+    "aaa"
+  ]
+  result: {
+    item: "allthetweaks:greg_star_block"
+  }
+  show_notification: true
+}

```


</details>

<details>
<summary>allthetweaks/greg_star_from_gregstar_block</summary>

```diff
+{
+  type: "minecraft:crafting_shapeless"
+  category: "misc"
+  ingredients: [
+    {
+      tag: "forge:storage_blocks/greg_star"
+    }
+  ]
+  result: {
+    count: 9
+    item: "allthetweaks:greg_star"
+  }
+}

```


</details>

<details>
<summary>almostunified/createmoredrillheads</summary>

```diff
+{
+  type: "almostunified:client_recipe_tracker"
+  namespace: "createmoredrillheads"
+  recipes: [
+    "1$diamond_drill"
+    "1$netherite_drill"
+    "1$crushing/emerald"
+  ]
+}

```


</details>

<details>
<summary>create/kjs/9nbiqhksb0udukdx00y88q7po</summary>

```diff
+{
+  type: "create:cutting"
+  results: [
+    {
+      item: "immersiveengineering:slab_treated_wood_horizontal"
+      count: 2
+    }
+  ]
+  ingredients: [
+    {
+      item: "gtceu:treated_wood_planks"
+    }
+  ]
+  processingTime: 150
+}

```


</details>

<details>
<summary>createmoredrillheads/crushing/amethyst_shard</summary>

```diff
+{
+  type: "create:crushing"
+  ingredients: [
+    {
+      item: "minecraft:amethyst_shard"
+    }
+  ]
+  results: [
+    {
+      item: "createmoredrillheads:amethyst_dusts"
+      count: 1
+    }
+    {
+      item: "createmoredrillheads:amethyst_dusts"
+      chance: 0.5
+    }
+  ]
+  processingTime: 150
+}

```


</details>

<details>
<summary>createmoredrillheads/crushing/emerald</summary>

```diff
+{
+  type: "create:crushing"
+  ingredients: [
+    {
+      tag: "forge:gems/emerald"
+    }
+  ]
+  results: [
+    {
+      item: "gtceu:emerald_dust"
+      count: 1
+    }
+    {
+      item: "gtceu:emerald_dust"
+      chance: 0.5
+    }
+  ]
+  processingTime: 150
+}

```


</details>

<details>
<summary>createmoredrillheads/crushing/quartz</summary>

```diff
+{
+  type: "create:crushing"
+  ingredients: [
+    {
+      item: "minecraft:quartz"
+    }
+  ]
+  results: [
+    {
+      item: "createmoredrillheads:quartz_dusts"
+      count: 1
+    }
+    {
+      item: "createmoredrillheads:quartz_dusts"
+      chance: 0.5
+    }
+  ]
+  processingTime: 150
+}

```


</details>

<details>
<summary>createmoredrillheads/deploying/diamond_drill_amethyst_dusts_tip_attaching_recipe</summary>

```diff
+{
+  type: "create:deploying"
+  ingredients: [
+    {
+      item: "createmoredrillheads:diamond_drill"
+    }
+    {
+      tag: "forge:dusts/amethyst"
+    }
+  ]
+  results: [
+    {
+      item: "createmoredrillheads:amethyst_dusts_tipped_diamond_drill"
+    }
+  ]
+}

```


</details>

<details>
<summary>createmoredrillheads/deploying/diamond_drill_emerald_dusts_tip_attaching_recipe</summary>

```diff
+{
+  type: "create:deploying"
+  ingredients: [
+    {
+      item: "createmoredrillheads:diamond_drill"
+    }
+    {
+      tag: "forge:dusts/emerald"
+    }
+  ]
+  results: [
+    {
+      item: "createmoredrillheads:emerald_dusts_tipped_diamond_drill"
+    }
+  ]
+}

```


</details>

<details>
<summary>createmoredrillheads/deploying/diamond_drill_quartz_dusts_tip_attaching_recipe</summary>

```diff
+{
+  type: "create:deploying"
+  ingredients: [
+    {
+      item: "createmoredrillheads:diamond_drill"
+    }
+    {
+      tag: "forge:dusts/quartz"
+    }
+  ]
+  results: [
+    {
+      item: "createmoredrillheads:quartz_dusts_tipped_diamond_drill"
+    }
+  ]
+}

```


</details>

<details>
<summary>createmoredrillheads/deploying/diamond_drill_redstone_dusts_tip_attaching_recipe</summary>

```diff
+{
+  type: "create:deploying"
+  ingredients: [
+    {
+      item: "createmoredrillheads:diamond_drill"
+    }
+    {
+      tag: "forge:dusts/redstone"
+    }
+  ]
+  results: [
+    {
+      item: "createmoredrillheads:redstone_dusts_tipped_diamond_drill"
+    }
+  ]
+}

```


</details>

<details>
<summary>createmoredrillheads/deploying/gold_drill_amethyst_dusts_tip_attaching_recipe</summary>

```diff
+{
+  type: "create:deploying"
+  ingredients: [
+    {
+      item: "createmoredrillheads:golden_drill"
+    }
+    {
+      tag: "forge:dusts/amethyst"
+    }
+  ]
+  results: [
+    {
+      item: "createmoredrillheads:amethyst_dusts_tipped_golden_drill"
+    }
+  ]
+}

```


</details>

<details>
<summary>createmoredrillheads/deploying/gold_drill_emerald_dusts_tip_attaching_recipe</summary>

```diff
+{
+  type: "create:deploying"
+  ingredients: [
+    {
+      item: "createmoredrillheads:golden_drill"
+    }
+    {
+      tag: "forge:dusts/emerald"
+    }
+  ]
+  results: [
+    {
+      item: "createmoredrillheads:emerald_dusts_tipped_golden_drill"
+    }
+  ]
+}

```


</details>

<details>
<summary>createmoredrillheads/deploying/gold_drill_quartz_dusts_tip_attaching_recipe</summary>

```diff
+{
+  type: "create:deploying"
+  ingredients: [
+    {
+      item: "createmoredrillheads:golden_drill"
+    }
+    {
+      tag: "forge:dusts/quartz"
+    }
+  ]
+  results: [
+    {
+      item: "createmoredrillheads:quartz_dusts_tipped_golden_drill"
+    }
+  ]
+}

```


</details>

<details>
<summary>createmoredrillheads/deploying/gold_drill_redstone_dusts_tip_attaching_recipe</summary>

```diff
+{
+  type: "create:deploying"
+  ingredients: [
+    {
+      item: "createmoredrillheads:golden_drill"
+    }
+    {
+      tag: "forge:dusts/redstone"
+    }
+  ]
+  results: [
+    {
+      item: "createmoredrillheads:redstone_dusts_tipped_golden_drill"
+    }
+  ]
+}

```


</details>

<details>
<summary>createmoredrillheads/deploying/iron_drill_amethyst_dusts_tip_attaching_recipe</summary>

```diff
+{
+  type: "create:deploying"
+  ingredients: [
+    {
+      item: "createmoredrillheads:iron_drill"
+    }
+    {
+      tag: "forge:dusts/amethyst"
+    }
+  ]
+  results: [
+    {
+      item: "createmoredrillheads:amethyst_dusts_tipped_iron_drill"
+    }
+  ]
+}

```


</details>

<details>
<summary>createmoredrillheads/deploying/iron_drill_emerald_dusts_tip_attaching_recipe</summary>

```diff
+{
+  type: "create:deploying"
+  ingredients: [
+    {
+      item: "createmoredrillheads:iron_drill"
+    }
+    {
+      tag: "forge:dusts/emerald"
+    }
+  ]
+  results: [
+    {
+      item: "createmoredrillheads:emerald_dusts_tipped_iron_drill"
+    }
+  ]
+}

```


</details>

<details>
<summary>createmoredrillheads/deploying/iron_drill_quartz_dusts_tip_attaching_recipe</summary>

```diff
+{
+  type: "create:deploying"
+  ingredients: [
+    {
+      item: "createmoredrillheads:iron_drill"
+    }
+    {
+      tag: "forge:dusts/quartz"
+    }
+  ]
+  results: [
+    {
+      item: "createmoredrillheads:quartz_dusts_tipped_iron_drill"
+    }
+  ]
+}

```


</details>

<details>
<summary>createmoredrillheads/deploying/iron_drill_redstone_dusts_tip_attaching_recipe</summary>

```diff
+{
+  type: "create:deploying"
+  ingredients: [
+    {
+      item: "createmoredrillheads:iron_drill"
+    }
+    {
+      tag: "forge:dusts/redstone"
+    }
+  ]
+  results: [
+    {
+      item: "createmoredrillheads:redstone_dusts_tipped_iron_drill"
+    }
+  ]
+}

```


</details>

<details>
<summary>createmoredrillheads/deploying/netherite_drill_amethyst_dusts_tip_attaching_recipe</summary>

```diff
+{
+  type: "create:deploying"
+  ingredients: [
+    {
+      item: "createmoredrillheads:netherite_drill"
+    }
+    {
+      tag: "forge:dusts/amethyst"
+    }
+  ]
+  results: [
+    {
+      item: "createmoredrillheads:amethyst_dusts_tipped_netherite_drill"
+    }
+  ]
+}

```


</details>

<details>
<summary>createmoredrillheads/deploying/netherite_drill_emerald_dusts_tip_attaching_recipe</summary>

```diff
+{
+  type: "create:deploying"
+  ingredients: [
+    {
+      item: "createmoredrillheads:netherite_drill"
+    }
+    {
+      tag: "forge:dusts/emerald"
+    }
+  ]
+  results: [
+    {
+      item: "createmoredrillheads:emerald_dusts_tipped_netherite_drill"
+    }
+  ]
+}

```


</details>

<details>
<summary>createmoredrillheads/deploying/netherite_drill_quartz_dusts_tip_attaching_recipe</summary>

```diff
+{
+  type: "create:deploying"
+  ingredients: [
+    {
+      item: "createmoredrillheads:netherite_drill"
+    }
+    {
+      tag: "forge:dusts/quartz"
+    }
+  ]
+  results: [
+    {
+      item: "createmoredrillheads:quartz_dusts_tipped_netherite_drill"
+    }
+  ]
+}

```


</details>

<details>
<summary>createmoredrillheads/deploying/netherite_drill_redstone_dusts_tip_attaching_recipe</summary>

```diff
+{
+  type: "create:deploying"
+  ingredients: [
+    {
+      item: "createmoredrillheads:netherite_drill"
+    }
+    {
+      tag: "forge:dusts/redstone"
+    }
+  ]
+  results: [
+    {
+      item: "createmoredrillheads:redstone_dusts_tipped_netherite_drill"
+    }
+  ]
+}

```


</details>

<details>
<summary>createmoredrillheads/deploying/stone_drill_amethyst_dusts_tip_attaching_recipe</summary>

```diff
+{
+  type: "create:deploying"
+  ingredients: [
+    {
+      item: "createmoredrillheads:stone_drill"
+    }
+    {
+      tag: "forge:dusts/amethyst"
+    }
+  ]
+  results: [
+    {
+      item: "createmoredrillheads:amethyst_dusts_tipped_stone_drill"
+    }
+  ]
+}

```


</details>

<details>
<summary>createmoredrillheads/deploying/stone_drill_emerald_dusts_tip_attaching_recipe</summary>

```diff
+{
+  type: "create:deploying"
+  ingredients: [
+    {
+      item: "createmoredrillheads:stone_drill"
+    }
+    {
+      tag: "forge:dusts/emerald"
+    }
+  ]
+  results: [
+    {
+      item: "createmoredrillheads:emerald_dusts_tipped_stone_drill"
+    }
+  ]
+}

```


</details>

<details>
<summary>createmoredrillheads/deploying/stone_drill_quartz_dusts_tip_attaching_recipe</summary>

```diff
+{
+  type: "create:deploying"
+  ingredients: [
+    {
+      item: "createmoredrillheads:stone_drill"
+    }
+    {
+      tag: "forge:dusts/quartz"
+    }
+  ]
+  results: [
+    {
+      item: "createmoredrillheads:quartz_dusts_tipped_stone_drill"
+    }
+  ]
+}

```


</details>

<details>
<summary>createmoredrillheads/deploying/stone_drill_redstone_dusts_tip_attaching_recipe</summary>

```diff
+{
+  type: "create:deploying"
+  ingredients: [
+    {
+      item: "createmoredrillheads:stone_drill"
+    }
+    {
+      tag: "forge:dusts/redstone"
+    }
+  ]
+  results: [
+    {
+      item: "createmoredrillheads:redstone_dusts_tipped_stone_drill"
+    }
+  ]
+}

```


</details>

<details>
<summary>createmoredrillheads/deploying/wood_drill_amethyst_dusts_tip_attaching_recipe</summary>

```diff
+{
+  type: "create:deploying"
+  ingredients: [
+    {
+      item: "createmoredrillheads:wooden_drill"
+    }
+    {
+      tag: "forge:dusts/amethyst"
+    }
+  ]
+  results: [
+    {
+      item: "createmoredrillheads:amethyst_dusts_tipped_wooden_drill"
+    }
+  ]
+}

```


</details>

<details>
<summary>createmoredrillheads/deploying/wood_drill_emerald_dusts_tip_attaching_recipe</summary>

```diff
+{
+  type: "create:deploying"
+  ingredients: [
+    {
+      item: "createmoredrillheads:wooden_drill"
+    }
+    {
+      tag: "forge:dusts/emerald"
+    }
+  ]
+  results: [
+    {
+      item: "createmoredrillheads:emerald_dusts_tipped_wooden_drill"
+    }
+  ]
+}

```


</details>

<details>
<summary>createmoredrillheads/deploying/wood_drill_quartz_dusts_tip_attaching_recipe</summary>

```diff
+{
+  type: "create:deploying"
+  ingredients: [
+    {
+      item: "createmoredrillheads:wooden_drill"
+    }
+    {
+      tag: "forge:dusts/quartz"
+    }
+  ]
+  results: [
+    {
+      item: "createmoredrillheads:quartz_dusts_tipped_wooden_drill"
+    }
+  ]
+}

```


</details>

<details>
<summary>createmoredrillheads/deploying/wood_drill_redstone_dusts_tip_attaching_recipe</summary>

```diff
+{
+  type: "create:deploying"
+  ingredients: [
+    {
+      item: "createmoredrillheads:wooden_drill"
+    }
+    {
+      tag: "forge:dusts/redstone"
+    }
+  ]
+  results: [
+    {
+      item: "createmoredrillheads:redstone_dusts_tipped_wooden_drill"
+    }
+  ]
+}

```


</details>

<details>
<summary>createmoredrillheads/diamond_drill</summary>

```diff
+{
+  type: "minecraft:crafting_shaped"
+  pattern: [
+    " A "
+    "AIA"
+    " C "
+  ]
+  key: {
+    C: {
+      item: "create:andesite_casing"
+    }
+    A: {
+      tag: "forge:gems/diamond"
+    }
+    I: {
+      tag: "forge:ingots/iron"
+    }
+  }
+  result: {
+    item: "createmoredrillheads:diamond_drill"
+  }
+}

```


</details>

<details>
<summary>createmoredrillheads/golden_drill</summary>

```diff
+{
+  type: "minecraft:crafting_shaped"
+  pattern: [
+    " A "
+    "AIA"
+    " C "
+  ]
+  key: {
+    C: {
+      item: "create:andesite_casing"
+    }
+    A: {
+      tag: "forge:ingots/gold"
+    }
+    I: {
+      tag: "forge:ingots/iron"
+    }
+  }
+  result: {
+    item: "createmoredrillheads:golden_drill"
+  }
+}

```


</details>

<details>
<summary>createmoredrillheads/iron_drill</summary>

```diff
+{
+  type: "minecraft:crafting_shaped"
+  pattern: [
+    " I "
+    "III"
+    " C "
+  ]
+  key: {
+    C: {
+      item: "create:andesite_casing"
+    }
+    I: {
+      tag: "forge:ingots/iron"
+    }
+  }
+  result: {
+    item: "createmoredrillheads:iron_drill"
+  }
+}

```


</details>

<details>
<summary>createmoredrillheads/netherite_drill</summary>

```diff
+{
+  type: "minecraft:smithing_transform"
+  base: {
+    item: "createmoredrillheads:diamond_drill"
+  }
+  addition: {
+    tag: "forge:ingots/netherite"
+  }
+  result: {
+    item: "createmoredrillheads:netherite_drill"
+  }
+  template: {
+    item: "minecraft:netherite_upgrade_smithing_template"
+  }
+}

```


</details>

<details>
<summary>createmoredrillheads/stone_drill</summary>

```diff
+{
+  type: "minecraft:crafting_shaped"
+  pattern: [
+    " A "
+    "AIA"
+    " C "
+  ]
+  key: {
+    C: {
+      item: "create:andesite_casing"
+    }
+    A: {
+      tag: "minecraft:stone_tool_materials"
+    }
+    I: {
+      tag: "forge:ingots/iron"
+    }
+  }
+  result: {
+    item: "createmoredrillheads:stone_drill"
+  }
+}

```


</details>

<details>
<summary>createmoredrillheads/wooden_drill</summary>

```diff
+{
+  type: "minecraft:crafting_shaped"
+  pattern: [
+    " T "
+    "AIA"
+    " C "
+  ]
+  key: {
+    C: {
+      item: "create:andesite_casing"
+    }
+    A: {
+      tag: "minecraft:planks"
+    }
+    I: {
+      tag: "forge:ingots/iron"
+    }
+    T: {
+      tag: "minecraft:logs"
+    }
+  }
+  result: {
+    item: "createmoredrillheads:wooden_drill"
+  }
+}

```


</details>

<details>
<summary>gtceu/alloy_smelter/igneous_alloy</summary>

```diff
+{
+  type: "gtceu:alloy_smelter"
+  duration: 60
+  inputs: {
+    item: [
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gregitas_core:igneous_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:small_zinc_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+    ]
+  }
+  tickInputs: {
+    eu: [
+      {
+        content: 30
+        chance: 1
+        tierChanceBoost: 0
+      }
+    ]
+  }
+  outputs: {
+    item: [
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 1
+          ingredient: {
+            item: "create:andesite_alloy"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+    ]
+  }
+}

```


</details>

<details>
<summary>gtceu/extractor/extract_glass_lens</summary>

```diff
+{
+  type: "gtceu:extractor"
+  duration: 15
+  inputs: {
+    item: [
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 1
+          ingredient: {
+            tag: "forge:lenses/glass"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+    ]
+  }
+  outputs: {
+    fluid: [
+      {
+        content: {
+          amount: 108
+          value: [
+            {
+              fluid: "gtceu:glass"
+            }
+          ]
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+    ]
+  }
+  tickInputs: {
+    eu: [
+      {
+        content: 30
+        chance: 1
+        tierChanceBoost: 0
+      }
+    ]
+  }
+  tickOutputs: {
+  }
+}

```


</details>

<details>
<summary>gtceu/macerator/andesite_dust</summary>

```diff
+{
+  type: "gtceu:macerator"
+  duration: 60
+  inputs: {
+    item: [
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 1
+          ingredient: {
+            item: "tfc:rock/loose/andesite"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+    ]
+  }
+  tickInputs: {
+    eu: [
+      {
+        content: 30
+        chance: 1
+        tierChanceBoost: 0
+      }
+    ]
+  }
+  outputs: {
+    item: [
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 1
+          ingredient: {
+            item: "gtceu:andesite_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 1
+          ingredient: {
+            item: "gtceu:andesite_dust"
+          }
+        }
+        chance: 0.1
+        tierChanceBoost: 0.0001
+      }
+    ]
+  }
+}

```


</details>

<details>
<summary>gtceu/macerator/basalt_dust</summary>

```diff
+{
+  type: "gtceu:macerator"
+  duration: 60
+  inputs: {
+    item: [
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 1
+          ingredient: {
+            item: "tfc:rock/loose/basalt"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+    ]
+  }
+  tickInputs: {
+    eu: [
+      {
+        content: 30
+        chance: 1
+        tierChanceBoost: 0
+      }
+    ]
+  }
+  outputs: {
+    item: [
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 1
+          ingredient: {
+            item: "gtceu:basalt_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 1
+          ingredient: {
+            item: "gtceu:basalt_dust"
+          }
+        }
+        chance: 0.1
+        tierChanceBoost: 0.0001
+      }
+    ]
+  }
+}

```


</details>

<details>
<summary>gtceu/macerator/chalk_dust</summary>

```diff
+{
+  type: "gtceu:macerator"
+  duration: 60
+  inputs: {
+    item: [
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 1
+          ingredient: {
+            item: "tfc:rock/loose/chalk"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+    ]
+  }
+  tickInputs: {
+    eu: [
+      {
+        content: 30
+        chance: 1
+        tierChanceBoost: 0
+      }
+    ]
+  }
+  outputs: {
+    item: [
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 1
+          ingredient: {
+            item: "gregitas_core:chalk_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 1
+          ingredient: {
+            item: "gregitas_core:chalk_dust"
+          }
+        }
+        chance: 0.1
+        tierChanceBoost: 0.0001
+      }
+    ]
+  }
+}

```


</details>

<details>
<summary>gtceu/macerator/chert_dust</summary>

```diff
+{
+  type: "gtceu:macerator"
+  duration: 60
+  inputs: {
+    item: [
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 1
+          ingredient: {
+            item: "tfc:rock/loose/chert"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+    ]
+  }
+  tickInputs: {
+    eu: [
+      {
+        content: 30
+        chance: 1
+        tierChanceBoost: 0
+      }
+    ]
+  }
+  outputs: {
+    item: [
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 1
+          ingredient: {
+            item: "gregitas_core:chert_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 1
+          ingredient: {
+            item: "gregitas_core:chert_dust"
+          }
+        }
+        chance: 0.1
+        tierChanceBoost: 0.0001
+      }
+    ]
+  }
+}

```


</details>

<details>
<summary>gtceu/macerator/claystone_dust</summary>

```diff
+{
+  type: "gtceu:macerator"
+  duration: 60
+  inputs: {
+    item: [
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 1
+          ingredient: {
+            item: "tfc:rock/loose/claystone"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+    ]
+  }
+  tickInputs: {
+    eu: [
+      {
+        content: 30
+        chance: 1
+        tierChanceBoost: 0
+      }
+    ]
+  }
+  outputs: {
+    item: [
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 1
+          ingredient: {
+            item: "gregitas_core:claystone_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 1
+          ingredient: {
+            item: "gregitas_core:claystone_dust"
+          }
+        }
+        chance: 0.1
+        tierChanceBoost: 0.0001
+      }
+    ]
+  }
+}

```


</details>

<details>
<summary>gtceu/macerator/conglomerate_dust</summary>

```diff
+{
+  type: "gtceu:macerator"
+  duration: 60
+  inputs: {
+    item: [
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 1
+          ingredient: {
+            item: "tfc:rock/loose/conglomerate"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+    ]
+  }
+  tickInputs: {
+    eu: [
+      {
+        content: 30
+        chance: 1
+        tierChanceBoost: 0
+      }
+    ]
+  }
+  outputs: {
+    item: [
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 1
+          ingredient: {
+            item: "gregitas_core:conglomerate_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 1
+          ingredient: {
+            item: "gregitas_core:conglomerate_dust"
+          }
+        }
+        chance: 0.1
+        tierChanceBoost: 0.0001
+      }
+    ]
+  }
+}

```


</details>

<details>
<summary>gtceu/macerator/dacite_dust</summary>

```diff
+{
+  type: "gtceu:macerator"
+  duration: 60
+  inputs: {
+    item: [
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 1
+          ingredient: {
+            item: "tfc:rock/loose/dacite"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+    ]
+  }
+  tickInputs: {
+    eu: [
+      {
+        content: 30
+        chance: 1
+        tierChanceBoost: 0
+      }
+    ]
+  }
+  outputs: {
+    item: [
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 1
+          ingredient: {
+            item: "gregitas_core:dacite_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 1
+          ingredient: {
+            item: "gregitas_core:dacite_dust"
+          }
+        }
+        chance: 0.1
+        tierChanceBoost: 0.0001
+      }
+    ]
+  }
+}

```


</details>

<details>
<summary>gtceu/macerator/diorite_dust</summary>

```diff
+{
+  type: "gtceu:macerator"
+  duration: 60
+  inputs: {
+    item: [
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 1
+          ingredient: {
+            item: "tfc:rock/loose/diorite"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+    ]
+  }
+  tickInputs: {
+    eu: [
+      {
+        content: 30
+        chance: 1
+        tierChanceBoost: 0
+      }
+    ]
+  }
+  outputs: {
+    item: [
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 1
+          ingredient: {
+            item: "gtceu:diorite_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 1
+          ingredient: {
+            item: "gtceu:diorite_dust"
+          }
+        }
+        chance: 0.1
+        tierChanceBoost: 0.0001
+      }
+    ]
+  }
+}

```


</details>

<details>
<summary>gtceu/macerator/dolomite_dust</summary>

```diff
+{
+  type: "gtceu:macerator"
+  duration: 60
+  inputs: {
+    item: [
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 1
+          ingredient: {
+            item: "tfc:rock/loose/dolomite"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+    ]
+  }
+  tickInputs: {
+    eu: [
+      {
+        content: 30
+        chance: 1
+        tierChanceBoost: 0
+      }
+    ]
+  }
+  outputs: {
+    item: [
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 1
+          ingredient: {
+            item: "gregitas_core:dolomite_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 1
+          ingredient: {
+            item: "gregitas_core:dolomite_dust"
+          }
+        }
+        chance: 0.1
+        tierChanceBoost: 0.0001
+      }
+    ]
+  }
+}

```


</details>

<details>
<summary>gtceu/macerator/gabbro_dust</summary>

```diff
+{
+  type: "gtceu:macerator"
+  duration: 60
+  inputs: {
+    item: [
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 1
+          ingredient: {
+            item: "tfc:rock/loose/gabbro"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+    ]
+  }
+  tickInputs: {
+    eu: [
+      {
+        content: 30
+        chance: 1
+        tierChanceBoost: 0
+      }
+    ]
+  }
+  outputs: {
+    item: [
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 1
+          ingredient: {
+            item: "gregitas_core:gabbro_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 1
+          ingredient: {
+            item: "gregitas_core:gabbro_dust"
+          }
+        }
+        chance: 0.1
+        tierChanceBoost: 0.0001
+      }
+    ]
+  }
+}

```


</details>

<details>
<summary>gtceu/macerator/gneiss_dust</summary>

```diff
+{
+  type: "gtceu:macerator"
+  duration: 60
+  inputs: {
+    item: [
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 1
+          ingredient: {
+            item: "tfc:rock/loose/gneiss"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+    ]
+  }
+  tickInputs: {
+    eu: [
+      {
+        content: 30
+        chance: 1
+        tierChanceBoost: 0
+      }
+    ]
+  }
+  outputs: {
+    item: [
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 1
+          ingredient: {
+            item: "gregitas_core:gneiss_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 1
+          ingredient: {
+            item: "gregitas_core:gneiss_dust"
+          }
+        }
+        chance: 0.1
+        tierChanceBoost: 0.0001
+      }
+    ]
+  }
+}

```


</details>

<details>
<summary>gtceu/macerator/granite_dust</summary>

```diff
+{
+  type: "gtceu:macerator"
+  duration: 60
+  inputs: {
+    item: [
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 1
+          ingredient: {
+            item: "tfc:rock/loose/granite"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+    ]
+  }
+  tickInputs: {
+    eu: [
+      {
+        content: 30
+        chance: 1
+        tierChanceBoost: 0
+      }
+    ]
+  }
+  outputs: {
+    item: [
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 1
+          ingredient: {
+            item: "gtceu:granite_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 1
+          ingredient: {
+            item: "gtceu:granite_dust"
+          }
+        }
+        chance: 0.1
+        tierChanceBoost: 0.0001
+      }
+    ]
+  }
+}

```


</details>

<details>
<summary>gtceu/macerator/limestone_dust</summary>

```diff
+{
+  type: "gtceu:macerator"
+  duration: 60
+  inputs: {
+    item: [
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 1
+          ingredient: {
+            item: "tfc:rock/loose/limestone"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+    ]
+  }
+  tickInputs: {
+    eu: [
+      {
+        content: 30
+        chance: 1
+        tierChanceBoost: 0
+      }
+    ]
+  }
+  outputs: {
+    item: [
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 1
+          ingredient: {
+            item: "gregitas_core:limestone_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 1
+          ingredient: {
+            item: "gregitas_core:limestone_dust"
+          }
+        }
+        chance: 0.1
+        tierChanceBoost: 0.0001
+      }
+    ]
+  }
+}

```


</details>

<details>
<summary>gtceu/macerator/marble_dust</summary>

```diff
+{
+  type: "gtceu:macerator"
+  duration: 60
+  inputs: {
+    item: [
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 1
+          ingredient: {
+            item: "tfc:rock/loose/marble"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+    ]
+  }
+  tickInputs: {
+    eu: [
+      {
+        content: 30
+        chance: 1
+        tierChanceBoost: 0
+      }
+    ]
+  }
+  outputs: {
+    item: [
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 1
+          ingredient: {
+            item: "gtceu:marble_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 1
+          ingredient: {
+            item: "gtceu:marble_dust"
+          }
+        }
+        chance: 0.1
+        tierChanceBoost: 0.0001
+      }
+    ]
+  }
+}

```


</details>

<details>
<summary>gtceu/macerator/phyllite_dust</summary>

```diff
+{
+  type: "gtceu:macerator"
+  duration: 60
+  inputs: {
+    item: [
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 1
+          ingredient: {
+            item: "tfc:rock/loose/phyllite"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+    ]
+  }
+  tickInputs: {
+    eu: [
+      {
+        content: 30
+        chance: 1
+        tierChanceBoost: 0
+      }
+    ]
+  }
+  outputs: {
+    item: [
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 1
+          ingredient: {
+            item: "gregitas_core:phyllite_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 1
+          ingredient: {
+            item: "gregitas_core:phyllite_dust"
+          }
+        }
+        chance: 0.1
+        tierChanceBoost: 0.0001
+      }
+    ]
+  }
+}

```


</details>

<details>
<summary>gtceu/macerator/quartzite_dust</summary>

```diff
+{
+  type: "gtceu:macerator"
+  duration: 60
+  inputs: {
+    item: [
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 1
+          ingredient: {
+            item: "tfc:rock/loose/quartzite"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+    ]
+  }
+  tickInputs: {
+    eu: [
+      {
+        content: 30
+        chance: 1
+        tierChanceBoost: 0
+      }
+    ]
+  }
+  outputs: {
+    item: [
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 1
+          ingredient: {
+            item: "gtceu:quartzite_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 1
+          ingredient: {
+            item: "gtceu:quartzite_dust"
+          }
+        }
+        chance: 0.1
+        tierChanceBoost: 0.0001
+      }
+    ]
+  }
+}

```


</details>

<details>
<summary>gtceu/macerator/rhyolite_dust</summary>

```diff
+{
+  type: "gtceu:macerator"
+  duration: 60
+  inputs: {
+    item: [
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 1
+          ingredient: {
+            item: "tfc:rock/loose/rhyolite"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+    ]
+  }
+  tickInputs: {
+    eu: [
+      {
+        content: 30
+        chance: 1
+        tierChanceBoost: 0
+      }
+    ]
+  }
+  outputs: {
+    item: [
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 1
+          ingredient: {
+            item: "gregitas_core:rhyolite_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 1
+          ingredient: {
+            item: "gregitas_core:rhyolite_dust"
+          }
+        }
+        chance: 0.1
+        tierChanceBoost: 0.0001
+      }
+    ]
+  }
+}

```


</details>

<details>
<summary>gtceu/macerator/schist_dust</summary>

```diff
+{
+  type: "gtceu:macerator"
+  duration: 60
+  inputs: {
+    item: [
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 1
+          ingredient: {
+            item: "tfc:rock/loose/schist"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+    ]
+  }
+  tickInputs: {
+    eu: [
+      {
+        content: 30
+        chance: 1
+        tierChanceBoost: 0
+      }
+    ]
+  }
+  outputs: {
+    item: [
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 1
+          ingredient: {
+            item: "gregitas_core:schist_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 1
+          ingredient: {
+            item: "gregitas_core:schist_dust"
+          }
+        }
+        chance: 0.1
+        tierChanceBoost: 0.0001
+      }
+    ]
+  }
+}

```


</details>

<details>
<summary>gtceu/macerator/shale_dust</summary>

```diff
+{
+  type: "gtceu:macerator"
+  duration: 60
+  inputs: {
+    item: [
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 1
+          ingredient: {
+            item: "tfc:rock/loose/shale"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+    ]
+  }
+  tickInputs: {
+    eu: [
+      {
+        content: 30
+        chance: 1
+        tierChanceBoost: 0
+      }
+    ]
+  }
+  outputs: {
+    item: [
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 1
+          ingredient: {
+            item: "gregitas_core:shale_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 1
+          ingredient: {
+            item: "gregitas_core:shale_dust"
+          }
+        }
+        chance: 0.1
+        tierChanceBoost: 0.0001
+      }
+    ]
+  }
+}

```


</details>

<details>
<summary>gtceu/macerator/slate_dust</summary>

```diff
+{
+  type: "gtceu:macerator"
+  duration: 60
+  inputs: {
+    item: [
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 1
+          ingredient: {
+            item: "tfc:rock/loose/slate"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+    ]
+  }
+  tickInputs: {
+    eu: [
+      {
+        content: 30
+        chance: 1
+        tierChanceBoost: 0
+      }
+    ]
+  }
+  outputs: {
+    item: [
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 1
+          ingredient: {
+            item: "gregitas_core:slate_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 1
+          ingredient: {
+            item: "gregitas_core:slate_dust"
+          }
+        }
+        chance: 0.1
+        tierChanceBoost: 0.0001
+      }
+    ]
+  }
+}

```


</details>

<details>
<summary>mcw_tfc_aio/large_boiler/roofs/thatch2_roofs/thatch2_attic_roof</summary>

```diff
+{
+  type: "gtceu:large_boiler"
+  duration: 3
+  inputs: {
+    item: [
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 1
+          ingredient: {
+            item: "mcw_tfc_aio:roofs/thatch2_roofs/thatch2_attic_roof"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+    ]
+  }
+  outputs: {
+  }
+  tickInputs: {
+  }
+  tickOutputs: {
+  }
+}

```


</details>

<details>
<summary>mcw_tfc_aio/large_boiler/roofs/thatch2_roofs/thatch2_lower_roof</summary>

```diff
+{
+  type: "gtceu:large_boiler"
+  duration: 3
+  inputs: {
+    item: [
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 1
+          ingredient: {
+            item: "mcw_tfc_aio:roofs/thatch2_roofs/thatch2_lower_roof"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+    ]
+  }
+  outputs: {
+  }
+  tickInputs: {
+  }
+  tickOutputs: {
+  }
+}

```


</details>

<details>
<summary>mcw_tfc_aio/large_boiler/roofs/thatch2_roofs/thatch2_roof</summary>

```diff
+{
+  type: "gtceu:large_boiler"
+  duration: 3
+  inputs: {
+    item: [
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 1
+          ingredient: {
+            item: "mcw_tfc_aio:roofs/thatch2_roofs/thatch2_roof"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+    ]
+  }
+  outputs: {
+  }
+  tickInputs: {
+  }
+  tickOutputs: {
+  }
+}

```


</details>

<details>
<summary>mcw_tfc_aio/large_boiler/roofs/thatch2_roofs/thatch2_steep_roof</summary>

```diff
+{
+  type: "gtceu:large_boiler"
+  duration: 3
+  inputs: {
+    item: [
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 1
+          ingredient: {
+            item: "mcw_tfc_aio:roofs/thatch2_roofs/thatch2_steep_roof"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+    ]
+  }
+  outputs: {
+  }
+  tickInputs: {
+  }
+  tickOutputs: {
+  }
+}

```


</details>

<details>
<summary>mcw_tfc_aio/large_boiler/roofs/thatch2_roofs/thatch2_top_roof</summary>

```diff
+{
+  type: "gtceu:large_boiler"
+  duration: 3
+  inputs: {
+    item: [
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 1
+          ingredient: {
+            item: "mcw_tfc_aio:roofs/thatch2_roofs/thatch2_top_roof"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+    ]
+  }
+  outputs: {
+  }
+  tickInputs: {
+  }
+  tickOutputs: {
+  }
+}

```


</details>

<details>
<summary>mcw_tfc_aio/large_boiler/roofs/thatch2_roofs/thatch2_upper_lower_roof</summary>

```diff
+{
+  type: "gtceu:large_boiler"
+  duration: 3
+  inputs: {
+    item: [
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 1
+          ingredient: {
+            item: "mcw_tfc_aio:roofs/thatch2_roofs/thatch2_upper_lower_roof"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+    ]
+  }
+  outputs: {
+  }
+  tickInputs: {
+  }
+  tickOutputs: {
+  }
+}

```


</details>

<details>
<summary>mcw_tfc_aio/large_boiler/roofs/thatch2_roofs/thatch2_upper_steep_roof</summary>

```diff
+{
+  type: "gtceu:large_boiler"
+  duration: 3
+  inputs: {
+    item: [
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 1
+          ingredient: {
+            item: "mcw_tfc_aio:roofs/thatch2_roofs/thatch2_upper_steep_roof"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+    ]
+  }
+  outputs: {
+  }
+  tickInputs: {
+  }
+  tickOutputs: {
+  }
+}

```


</details>

<details>
<summary>mcw_tfc_aio/roofs/acacia_roofs/acacia_log_roof_uncraft</summary>

```diff
+{
+  type: "tfc:damage_inputs_shapeless_crafting"
+  recipe: {
+    type: "minecraft:crafting_shapeless"
+    ingredients: [
+      {
+        tag: "mcw_tfc_aio:acacia_log_roofs"
+      }
+      {
+        tag: "tfc:saws"
+      }
+    ]
+    result: {
+      item: "tfc:wood/log/acacia"
+      count: 1
+    }
+  }
+}

```


</details>

<details>
<summary>mcw_tfc_aio/roofs/acacia_roofs/acacia_plank_roof_uncraft</summary>

```diff
+{
+  type: "tfc:damage_inputs_shapeless_crafting"
+  recipe: {
+    type: "minecraft:crafting_shapeless"
+    ingredients: [
+      {
+        tag: "mcw_tfc_aio:acacia_planks_roofs"
+      }
+      {
+        tag: "tfc:saws"
+      }
+    ]
+    result: {
+      item: "tfc:wood/planks/acacia"
+      count: 1
+    }
+  }
+}

```


</details>

<details>
<summary>mcw_tfc_aio/roofs/ash_roofs/ash_log_roof_uncraft</summary>

```diff
+{
+  type: "tfc:damage_inputs_shapeless_crafting"
+  recipe: {
+    type: "minecraft:crafting_shapeless"
+    ingredients: [
+      {
+        tag: "mcw_tfc_aio:ash_log_roofs"
+      }
+      {
+        tag: "tfc:saws"
+      }
+    ]
+    result: {
+      item: "tfc:wood/log/ash"
+      count: 1
+    }
+  }
+}

```


</details>

<details>
<summary>mcw_tfc_aio/roofs/ash_roofs/ash_plank_roof_uncraft</summary>

```diff
+{
+  type: "tfc:damage_inputs_shapeless_crafting"
+  recipe: {
+    type: "minecraft:crafting_shapeless"
+    ingredients: [
+      {
+        tag: "mcw_tfc_aio:ash_planks_roofs"
+      }
+      {
+        tag: "tfc:saws"
+      }
+    ]
+    result: {
+      item: "tfc:wood/planks/ash"
+      count: 1
+    }
+  }
+}

```


</details>

<details>
<summary>mcw_tfc_aio/roofs/aspen_roofs/aspen_log_roof_uncraft</summary>

```diff
+{
+  type: "tfc:damage_inputs_shapeless_crafting"
+  recipe: {
+    type: "minecraft:crafting_shapeless"
+    ingredients: [
+      {
+        tag: "mcw_tfc_aio:aspen_log_roofs"
+      }
+      {
+        tag: "tfc:saws"
+      }
+    ]
+    result: {
+      item: "tfc:wood/log/aspen"
+      count: 1
+    }
+  }
+}

```


</details>

<details>
<summary>mcw_tfc_aio/roofs/aspen_roofs/aspen_plank_roof_uncraft</summary>

```diff
+{
+  type: "tfc:damage_inputs_shapeless_crafting"
+  recipe: {
+    type: "minecraft:crafting_shapeless"
+    ingredients: [
+      {
+        tag: "mcw_tfc_aio:aspen_planks_roofs"
+      }
+      {
+        tag: "tfc:saws"
+      }
+    ]
+    result: {
+      item: "tfc:wood/planks/aspen"
+      count: 1
+    }
+  }
+}

```


</details>

<details>
<summary>mcw_tfc_aio/roofs/base_roofs/base_roof_uncraft</summary>

```diff
+{
+  type: "tfc:damage_inputs_shapeless_crafting"
+  recipe: {
+    type: "minecraft:crafting_shapeless"
+    ingredients: [
+      {
+        tag: "mcw_tfc_aio:terracotta_roofs"
+      }
+      {
+        tag: "tfc:saws"
+      }
+    ]
+    result: {
+      item: "minecraft:terracotta"
+      count: 1
+    }
+  }
+}

```


</details>

<details>
<summary>mcw_tfc_aio/roofs/birch_roofs/birch_log_roof_uncraft</summary>

```diff
+{
+  type: "tfc:damage_inputs_shapeless_crafting"
+  recipe: {
+    type: "minecraft:crafting_shapeless"
+    ingredients: [
+      {
+        tag: "mcw_tfc_aio:birch_log_roofs"
+      }
+      {
+        tag: "tfc:saws"
+      }
+    ]
+    result: {
+      item: "tfc:wood/log/birch"
+      count: 1
+    }
+  }
+}

```


</details>

<details>
<summary>mcw_tfc_aio/roofs/birch_roofs/birch_plank_roof_uncraft</summary>

```diff
+{
+  type: "tfc:damage_inputs_shapeless_crafting"
+  recipe: {
+    type: "minecraft:crafting_shapeless"
+    ingredients: [
+      {
+        tag: "mcw_tfc_aio:birch_planks_roofs"
+      }
+      {
+        tag: "tfc:saws"
+      }
+    ]
+    result: {
+      item: "tfc:wood/planks/birch"
+      count: 1
+    }
+  }
+}

```


</details>

<details>
<summary>mcw_tfc_aio/roofs/black_concrete_roofs/black_concrete_roof_uncraft</summary>

```diff
+{
+  type: "tfc:damage_inputs_shapeless_crafting"
+  recipe: {
+    type: "minecraft:crafting_shapeless"
+    ingredients: [
+      {
+        tag: "mcw_tfc_aio:black_concrete_roofs"
+      }
+      {
+        tag: "tfc:saws"
+      }
+    ]
+    result: {
+      item: "minecraft:black_concrete"
+      count: 1
+    }
+  }
+}

```


</details>

<details>
<summary>mcw_tfc_aio/roofs/black_roofs/black_roof_uncraft</summary>

```diff
+{
+  type: "tfc:damage_inputs_shapeless_crafting"
+  recipe: {
+    type: "minecraft:crafting_shapeless"
+    ingredients: [
+      {
+        tag: "mcw_tfc_aio:black_roofs"
+      }
+      {
+        tag: "tfc:saws"
+      }
+    ]
+    result: {
+      item: "minecraft:black_terracotta"
+      count: 1
+    }
+  }
+}

```


</details>

<details>
<summary>mcw_tfc_aio/roofs/black_terracotta_roofs/black_terracotta_roof_uncraft</summary>

```diff
+{
+  type: "tfc:damage_inputs_shapeless_crafting"
+  recipe: {
+    type: "minecraft:crafting_shapeless"
+    ingredients: [
+      {
+        tag: "mcw_tfc_aio:black_terracotta_roofs"
+      }
+      {
+        tag: "tfc:saws"
+      }
+    ]
+    result: {
+      item: "minecraft:black_terracotta"
+      count: 1
+    }
+  }
+}

```


</details>

<details>
<summary>mcw_tfc_aio/roofs/blackwood_roofs/blackwood_log_roof_uncraft</summary>

```diff
+{
+  type: "tfc:damage_inputs_shapeless_crafting"
+  recipe: {
+    type: "minecraft:crafting_shapeless"
+    ingredients: [
+      {
+        tag: "mcw_tfc_aio:blackwood_log_roofs"
+      }
+      {
+        tag: "tfc:saws"
+      }
+    ]
+    result: {
+      item: "tfc:wood/log/blackwood"
+      count: 1
+    }
+  }
+}

```


</details>

<details>
<summary>mcw_tfc_aio/roofs/blackwood_roofs/blackwood_plank_roof_uncraft</summary>

```diff
+{
+  type: "tfc:damage_inputs_shapeless_crafting"
+  recipe: {
+    type: "minecraft:crafting_shapeless"
+    ingredients: [
+      {
+        tag: "mcw_tfc_aio:blackwood_planks_roofs"
+      }
+      {
+        tag: "tfc:saws"
+      }
+    ]
+    result: {
+      item: "tfc:wood/planks/blackwood"
+      count: 1
+    }
+  }
+}

```


</details>

<details>
<summary>mcw_tfc_aio/roofs/blue_concrete_roofs/blue_concrete_roof_uncraft</summary>

```diff
+{
+  type: "tfc:damage_inputs_shapeless_crafting"
+  recipe: {
+    type: "minecraft:crafting_shapeless"
+    ingredients: [
+      {
+        tag: "mcw_tfc_aio:blue_concrete_roofs"
+      }
+      {
+        tag: "tfc:saws"
+      }
+    ]
+    result: {
+      item: "minecraft:blue_concrete"
+      count: 1
+    }
+  }
+}

```


</details>

<details>
<summary>mcw_tfc_aio/roofs/blue_terracotta_roofs/blue_terracotta_roof_uncraft</summary>

```diff
+{
+  type: "tfc:damage_inputs_shapeless_crafting"
+  recipe: {
+    type: "minecraft:crafting_shapeless"
+    ingredients: [
+      {
+        tag: "mcw_tfc_aio:blue_terracotta_roofs"
+      }
+      {
+        tag: "tfc:saws"
+      }
+    ]
+    result: {
+      item: "minecraft:blue_terracotta"
+      count: 1
+    }
+  }
+}

```


</details>

<details>
<summary>mcw_tfc_aio/roofs/brick_roofs/bricks_roof_uncraft</summary>

```diff
+{
+  type: "tfc:damage_inputs_shapeless_crafting"
+  recipe: {
+    type: "minecraft:crafting_shapeless"
+    ingredients: [
+      {
+        tag: "mcw_tfc_aio:bricks_roofs"
+      }
+      {
+        tag: "tfc:saws"
+      }
+    ]
+    result: {
+      item: "minecraft:bricks"
+      count: 1
+    }
+  }
+}

```


</details>

<details>
<summary>mcw_tfc_aio/roofs/brown_concrete_roofs/brown_concrete_roof_uncraft</summary>

```diff
+{
+  type: "tfc:damage_inputs_shapeless_crafting"
+  recipe: {
+    type: "minecraft:crafting_shapeless"
+    ingredients: [
+      {
+        tag: "mcw_tfc_aio:brown_concrete_roofs"
+      }
+      {
+        tag: "tfc:saws"
+      }
+    ]
+    result: {
+      item: "minecraft:brown_concrete"
+      count: 1
+    }
+  }
+}

```


</details>

<details>
<summary>mcw_tfc_aio/roofs/brown_terracotta_roofs/brown_terracotta_roof_uncraft</summary>

```diff
+{
+  type: "tfc:damage_inputs_shapeless_crafting"
+  recipe: {
+    type: "minecraft:crafting_shapeless"
+    ingredients: [
+      {
+        tag: "mcw_tfc_aio:brown_terracotta_roofs"
+      }
+      {
+        tag: "tfc:saws"
+      }
+    ]
+    result: {
+      item: "minecraft:brown_terracotta"
+      count: 1
+    }
+  }
+}

```


</details>

<details>
<summary>mcw_tfc_aio/roofs/chestnut_roofs/chestnut_log_roof_uncraft</summary>

```diff
+{
+  type: "tfc:damage_inputs_shapeless_crafting"
+  recipe: {
+    type: "minecraft:crafting_shapeless"
+    ingredients: [
+      {
+        tag: "mcw_tfc_aio:chestnut_log_roofs"
+      }
+      {
+        tag: "tfc:saws"
+      }
+    ]
+    result: {
+      item: "tfc:wood/log/chestnut"
+      count: 1
+    }
+  }
+}

```


</details>

<details>
<summary>mcw_tfc_aio/roofs/chestnut_roofs/chestnut_plank_roof_uncraft</summary>

```diff
+{
+  type: "tfc:damage_inputs_shapeless_crafting"
+  recipe: {
+    type: "minecraft:crafting_shapeless"
+    ingredients: [
+      {
+        tag: "mcw_tfc_aio:chestnut_planks_roofs"
+      }
+      {
+        tag: "tfc:saws"
+      }
+    ]
+    result: {
+      item: "tfc:wood/planks/chestnut"
+      count: 1
+    }
+  }
+}

```


</details>

<details>
<summary>mcw_tfc_aio/roofs/cyan_concrete_roofs/cyan_concrete_roof_uncraft</summary>

```diff
+{
+  type: "tfc:damage_inputs_shapeless_crafting"
+  recipe: {
+    type: "minecraft:crafting_shapeless"
+    ingredients: [
+      {
+        tag: "mcw_tfc_aio:cyan_concrete_roofs"
+      }
+      {
+        tag: "tfc:saws"
+      }
+    ]
+    result: {
+      item: "minecraft:cyan_concrete"
+      count: 1
+    }
+  }
+}

```


</details>

<details>
<summary>mcw_tfc_aio/roofs/cyan_terracotta_roofs/cyan_terracotta_roof_uncraft</summary>

```diff
+{
+  type: "tfc:damage_inputs_shapeless_crafting"
+  recipe: {
+    type: "minecraft:crafting_shapeless"
+    ingredients: [
+      {
+        tag: "mcw_tfc_aio:cyan_terracotta_roofs"
+      }
+      {
+        tag: "tfc:saws"
+      }
+    ]
+    result: {
+      item: "minecraft:cyan_terracotta"
+      count: 1
+    }
+  }
+}

```


</details>

<details>
<summary>mcw_tfc_aio/roofs/douglas_fir_roofs/douglas_fir_log_roof_uncraft</summary>

```diff
+{
+  type: "tfc:damage_inputs_shapeless_crafting"
+  recipe: {
+    type: "minecraft:crafting_shapeless"
+    ingredients: [
+      {
+        tag: "mcw_tfc_aio:douglas_fir_log_roofs"
+      }
+      {
+        tag: "tfc:saws"
+      }
+    ]
+    result: {
+      item: "tfc:wood/log/douglas_fir"
+      count: 1
+    }
+  }
+}

```


</details>

<details>
<summary>mcw_tfc_aio/roofs/douglas_fir_roofs/douglas_fir_plank_roof_uncraft</summary>

```diff
+{
+  type: "tfc:damage_inputs_shapeless_crafting"
+  recipe: {
+    type: "minecraft:crafting_shapeless"
+    ingredients: [
+      {
+        tag: "mcw_tfc_aio:douglas_fir_planks_roofs"
+      }
+      {
+        tag: "tfc:saws"
+      }
+    ]
+    result: {
+      item: "tfc:wood/planks/douglas_fir"
+      count: 1
+    }
+  }
+}

```


</details>

<details>
<summary>mcw_tfc_aio/roofs/gray_concrete_roofs/gray_concrete_roof_uncraft</summary>

```diff
+{
+  type: "tfc:damage_inputs_shapeless_crafting"
+  recipe: {
+    type: "minecraft:crafting_shapeless"
+    ingredients: [
+      {
+        tag: "mcw_tfc_aio:gray_concrete_roofs"
+      }
+      {
+        tag: "tfc:saws"
+      }
+    ]
+    result: {
+      item: "minecraft:gray_concrete"
+      count: 1
+    }
+  }
+}

```


</details>

<details>
<summary>mcw_tfc_aio/roofs/gray_roofs/gray_roof_uncraft</summary>

```diff
+{
+  type: "tfc:damage_inputs_shapeless_crafting"
+  recipe: {
+    type: "minecraft:crafting_shapeless"
+    ingredients: [
+      {
+        tag: "mcw_tfc_aio:gray_roofs"
+      }
+      {
+        tag: "tfc:saws"
+      }
+    ]
+    result: {
+      item: "minecraft:gray_terracotta"
+      count: 1
+    }
+  }
+}

```


</details>

<details>
<summary>mcw_tfc_aio/roofs/gray_terracotta_roofs/gray_terracotta_roof_uncraft</summary>

```diff
+{
+  type: "tfc:damage_inputs_shapeless_crafting"
+  recipe: {
+    type: "minecraft:crafting_shapeless"
+    ingredients: [
+      {
+        tag: "mcw_tfc_aio:gray_terracotta_roofs"
+      }
+      {
+        tag: "tfc:saws"
+      }
+    ]
+    result: {
+      item: "minecraft:gray_terracotta"
+      count: 1
+    }
+  }
+}

```


</details>

<details>
<summary>mcw_tfc_aio/roofs/green_concrete_roofs/green_concrete_roof_uncraft</summary>

```diff
+{
+  type: "tfc:damage_inputs_shapeless_crafting"
+  recipe: {
+    type: "minecraft:crafting_shapeless"
+    ingredients: [
+      {
+        tag: "mcw_tfc_aio:green_concrete_roofs"
+      }
+      {
+        tag: "tfc:saws"
+      }
+    ]
+    result: {
+      item: "minecraft:green_concrete"
+      count: 1
+    }
+  }
+}

```


</details>

<details>
<summary>mcw_tfc_aio/roofs/green_terracotta_roofs/green_terracotta_roof_uncraft</summary>

```diff
+{
+  type: "tfc:damage_inputs_shapeless_crafting"
+  recipe: {
+    type: "minecraft:crafting_shapeless"
+    ingredients: [
+      {
+        tag: "mcw_tfc_aio:green_terracotta_roofs"
+      }
+      {
+        tag: "tfc:saws"
+      }
+    ]
+    result: {
+      item: "minecraft:green_terracotta"
+      count: 1
+    }
+  }
+}

```


</details>

<details>
<summary>mcw_tfc_aio/roofs/hickory_roofs/hickory_log_roof_uncraft</summary>

```diff
+{
+  type: "tfc:damage_inputs_shapeless_crafting"
+  recipe: {
+    type: "minecraft:crafting_shapeless"
+    ingredients: [
+      {
+        tag: "mcw_tfc_aio:hickory_log_roofs"
+      }
+      {
+        tag: "tfc:saws"
+      }
+    ]
+    result: {
+      item: "tfc:wood/log/hickory"
+      count: 1
+    }
+  }
+}

```


</details>

<details>
<summary>mcw_tfc_aio/roofs/hickory_roofs/hickory_plank_roof_uncraft</summary>

```diff
+{
+  type: "tfc:damage_inputs_shapeless_crafting"
+  recipe: {
+    type: "minecraft:crafting_shapeless"
+    ingredients: [
+      {
+        tag: "mcw_tfc_aio:hickory_planks_roofs"
+      }
+      {
+        tag: "tfc:saws"
+      }
+    ]
+    result: {
+      item: "tfc:wood/planks/hickory"
+      count: 1
+    }
+  }
+}

```


</details>

<details>
<summary>mcw_tfc_aio/roofs/kapok_roofs/kapok_log_roof_uncraft</summary>

```diff
+{
+  type: "tfc:damage_inputs_shapeless_crafting"
+  recipe: {
+    type: "minecraft:crafting_shapeless"
+    ingredients: [
+      {
+        tag: "mcw_tfc_aio:kapok_log_roofs"
+      }
+      {
+        tag: "tfc:saws"
+      }
+    ]
+    result: {
+      item: "tfc:wood/log/kapok"
+      count: 1
+    }
+  }
+}

```


</details>

<details>
<summary>mcw_tfc_aio/roofs/kapok_roofs/kapok_plank_roof_uncraft</summary>

```diff
+{
+  type: "tfc:damage_inputs_shapeless_crafting"
+  recipe: {
+    type: "minecraft:crafting_shapeless"
+    ingredients: [
+      {
+        tag: "mcw_tfc_aio:kapok_planks_roofs"
+      }
+      {
+        tag: "tfc:saws"
+      }
+    ]
+    result: {
+      item: "tfc:wood/planks/kapok"
+      count: 1
+    }
+  }
+}

```


</details>

<details>
<summary>mcw_tfc_aio/roofs/light_blue_concrete_roofs/light_blue_concrete_roof_uncraft</summary>

```diff
+{
+  type: "tfc:damage_inputs_shapeless_crafting"
+  recipe: {
+    type: "minecraft:crafting_shapeless"
+    ingredients: [
+      {
+        tag: "mcw_tfc_aio:light_blue_concrete_roofs"
+      }
+      {
+        tag: "tfc:saws"
+      }
+    ]
+    result: {
+      item: "minecraft:light_blue_concrete"
+      count: 1
+    }
+  }
+}

```


</details>

<details>
<summary>mcw_tfc_aio/roofs/light_blue_terracotta_roofs/light_blue_terracotta_roof_uncraft</summary>

```diff
+{
+  type: "tfc:damage_inputs_shapeless_crafting"
+  recipe: {
+    type: "minecraft:crafting_shapeless"
+    ingredients: [
+      {
+        tag: "mcw_tfc_aio:light_blue_terracotta_roofs"
+      }
+      {
+        tag: "tfc:saws"
+      }
+    ]
+    result: {
+      item: "minecraft:light_blue_terracotta"
+      count: 1
+    }
+  }
+}

```


</details>

<details>
<summary>mcw_tfc_aio/roofs/light_gray_concrete_roofs/light_gray_concrete_roof_uncraft</summary>

```diff
+{
+  type: "tfc:damage_inputs_shapeless_crafting"
+  recipe: {
+    type: "minecraft:crafting_shapeless"
+    ingredients: [
+      {
+        tag: "mcw_tfc_aio:light_gray_concrete_roofs"
+      }
+      {
+        tag: "tfc:saws"
+      }
+    ]
+    result: {
+      item: "minecraft:light_gray_concrete"
+      count: 1
+    }
+  }
+}

```


</details>

<details>
<summary>mcw_tfc_aio/roofs/light_gray_roofs/light_gray_roof_uncraft</summary>

```diff
+{
+  type: "tfc:damage_inputs_shapeless_crafting"
+  recipe: {
+    type: "minecraft:crafting_shapeless"
+    ingredients: [
+      {
+        tag: "mcw_tfc_aio:light_gray_roofs"
+      }
+      {
+        tag: "tfc:saws"
+      }
+    ]
+    result: {
+      item: "minecraft:light_gray_terracotta"
+      count: 1
+    }
+  }
+}

```


</details>

<details>
<summary>mcw_tfc_aio/roofs/light_gray_terracotta_roofs/light_gray_terracotta_roof_uncraft</summary>

```diff
+{
+  type: "tfc:damage_inputs_shapeless_crafting"
+  recipe: {
+    type: "minecraft:crafting_shapeless"
+    ingredients: [
+      {
+        tag: "mcw_tfc_aio:light_gray_terracotta_roofs"
+      }
+      {
+        tag: "tfc:saws"
+      }
+    ]
+    result: {
+      item: "minecraft:light_gray_terracotta"
+      count: 1
+    }
+  }
+}

```


</details>

<details>
<summary>mcw_tfc_aio/roofs/lime_concrete_roofs/lime_concrete_roof_uncraft</summary>

```diff
+{
+  type: "tfc:damage_inputs_shapeless_crafting"
+  recipe: {
+    type: "minecraft:crafting_shapeless"
+    ingredients: [
+      {
+        tag: "mcw_tfc_aio:lime_concrete_roofs"
+      }
+      {
+        tag: "tfc:saws"
+      }
+    ]
+    result: {
+      item: "minecraft:lime_concrete"
+      count: 1
+    }
+  }
+}

```


</details>

<details>
<summary>mcw_tfc_aio/roofs/lime_terracotta_roofs/lime_terracotta_roof_uncraft</summary>

```diff
+{
+  type: "tfc:damage_inputs_shapeless_crafting"
+  recipe: {
+    type: "minecraft:crafting_shapeless"
+    ingredients: [
+      {
+        tag: "mcw_tfc_aio:lime_terracotta_roofs"
+      }
+      {
+        tag: "tfc:saws"
+      }
+    ]
+    result: {
+      item: "minecraft:lime_terracotta"
+      count: 1
+    }
+  }
+}

```


</details>

<details>
<summary>mcw_tfc_aio/roofs/magenta_concrete_roofs/magenta_concrete_roof_uncraft</summary>

```diff
+{
+  type: "tfc:damage_inputs_shapeless_crafting"
+  recipe: {
+    type: "minecraft:crafting_shapeless"
+    ingredients: [
+      {
+        tag: "mcw_tfc_aio:magenta_concrete_roofs"
+      }
+      {
+        tag: "tfc:saws"
+      }
+    ]
+    result: {
+      item: "minecraft:magenta_concrete"
+      count: 1
+    }
+  }
+}

```


</details>

<details>
<summary>mcw_tfc_aio/roofs/magenta_terracotta_roofs/magenta_terracotta_roof_uncraft</summary>

```diff
+{
+  type: "tfc:damage_inputs_shapeless_crafting"
+  recipe: {
+    type: "minecraft:crafting_shapeless"
+    ingredients: [
+      {
+        tag: "mcw_tfc_aio:magenta_terracotta_roofs"
+      }
+      {
+        tag: "tfc:saws"
+      }
+    ]
+    result: {
+      item: "minecraft:magenta_terracotta"
+      count: 1
+    }
+  }
+}

```


</details>

<details>
<summary>mcw_tfc_aio/roofs/mangrove_roofs/mangrove_log_roof_uncraft</summary>

```diff
+{
+  type: "tfc:damage_inputs_shapeless_crafting"
+  recipe: {
+    type: "minecraft:crafting_shapeless"
+    ingredients: [
+      {
+        tag: "mcw_tfc_aio:mangrove_log_roofs"
+      }
+      {
+        tag: "tfc:saws"
+      }
+    ]
+    result: {
+      item: "tfc:wood/log/mangrove"
+      count: 1
+    }
+  }
+}

```


</details>

<details>
<summary>mcw_tfc_aio/roofs/mangrove_roofs/mangrove_plank_roof_uncraft</summary>

```diff
+{
+  type: "tfc:damage_inputs_shapeless_crafting"
+  recipe: {
+    type: "minecraft:crafting_shapeless"
+    ingredients: [
+      {
+        tag: "mcw_tfc_aio:mangrove_planks_roofs"
+      }
+      {
+        tag: "tfc:saws"
+      }
+    ]
+    result: {
+      item: "tfc:wood/planks/mangrove"
+      count: 1
+    }
+  }
+}

```


</details>

<details>
<summary>mcw_tfc_aio/roofs/maple_roofs/maple_log_roof_uncraft</summary>

```diff
+{
+  type: "tfc:damage_inputs_shapeless_crafting"
+  recipe: {
+    type: "minecraft:crafting_shapeless"
+    ingredients: [
+      {
+        tag: "mcw_tfc_aio:maple_log_roofs"
+      }
+      {
+        tag: "tfc:saws"
+      }
+    ]
+    result: {
+      item: "tfc:wood/log/maple"
+      count: 1
+    }
+  }
+}

```


</details>

<details>
<summary>mcw_tfc_aio/roofs/maple_roofs/maple_plank_roof_uncraft</summary>

```diff
+{
+  type: "tfc:damage_inputs_shapeless_crafting"
+  recipe: {
+    type: "minecraft:crafting_shapeless"
+    ingredients: [
+      {
+        tag: "mcw_tfc_aio:maple_planks_roofs"
+      }
+      {
+        tag: "tfc:saws"
+      }
+    ]
+    result: {
+      item: "tfc:wood/planks/maple"
+      count: 1
+    }
+  }
+}

```


</details>

<details>
<summary>mcw_tfc_aio/roofs/oak_roofs/oak_log_roof_uncraft</summary>

```diff
+{
+  type: "tfc:damage_inputs_shapeless_crafting"
+  recipe: {
+    type: "minecraft:crafting_shapeless"
+    ingredients: [
+      {
+        tag: "mcw_tfc_aio:oak_log_roofs"
+      }
+      {
+        tag: "tfc:saws"
+      }
+    ]
+    result: {
+      item: "tfc:wood/log/oak"
+      count: 1
+    }
+  }
+}

```


</details>

<details>
<summary>mcw_tfc_aio/roofs/oak_roofs/oak_plank_roof_uncraft</summary>

```diff
+{
+  type: "tfc:damage_inputs_shapeless_crafting"
+  recipe: {
+    type: "minecraft:crafting_shapeless"
+    ingredients: [
+      {
+        tag: "mcw_tfc_aio:oak_planks_roofs"
+      }
+      {
+        tag: "tfc:saws"
+      }
+    ]
+    result: {
+      item: "tfc:wood/planks/oak"
+      count: 1
+    }
+  }
+}

```


</details>

<details>
<summary>mcw_tfc_aio/roofs/orange_concrete_roofs/orange_concrete_roof_uncraft</summary>

```diff
+{
+  type: "tfc:damage_inputs_shapeless_crafting"
+  recipe: {
+    type: "minecraft:crafting_shapeless"
+    ingredients: [
+      {
+        tag: "mcw_tfc_aio:orange_concrete_roofs"
+      }
+      {
+        tag: "tfc:saws"
+      }
+    ]
+    result: {
+      item: "minecraft:orange_concrete"
+      count: 1
+    }
+  }
+}

```


</details>

<details>
<summary>mcw_tfc_aio/roofs/orange_terracotta_roofs/orange_terracotta_roof_uncraft</summary>

```diff
+{
+  type: "tfc:damage_inputs_shapeless_crafting"
+  recipe: {
+    type: "minecraft:crafting_shapeless"
+    ingredients: [
+      {
+        tag: "mcw_tfc_aio:orange_terracotta_roofs"
+      }
+      {
+        tag: "tfc:saws"
+      }
+    ]
+    result: {
+      item: "minecraft:orange_terracotta"
+      count: 1
+    }
+  }
+}

```


</details>

<details>
<summary>mcw_tfc_aio/roofs/palm_roofs/palm_log_roof_uncraft</summary>

```diff
+{
+  type: "tfc:damage_inputs_shapeless_crafting"
+  recipe: {
+    type: "minecraft:crafting_shapeless"
+    ingredients: [
+      {
+        tag: "mcw_tfc_aio:palm_log_roofs"
+      }
+      {
+        tag: "tfc:saws"
+      }
+    ]
+    result: {
+      item: "tfc:wood/log/palm"
+      count: 1
+    }
+  }
+}

```


</details>

<details>
<summary>mcw_tfc_aio/roofs/palm_roofs/palm_plank_roof_uncraft</summary>

```diff
+{
+  type: "tfc:damage_inputs_shapeless_crafting"
+  recipe: {
+    type: "minecraft:crafting_shapeless"
+    ingredients: [
+      {
+        tag: "mcw_tfc_aio:palm_planks_roofs"
+      }
+      {
+        tag: "tfc:saws"
+      }
+    ]
+    result: {
+      item: "tfc:wood/planks/palm"
+      count: 1
+    }
+  }
+}

```


</details>

<details>
<summary>mcw_tfc_aio/roofs/pine_roofs/pine_log_roof_uncraft</summary>

```diff
+{
+  type: "tfc:damage_inputs_shapeless_crafting"
+  recipe: {
+    type: "minecraft:crafting_shapeless"
+    ingredients: [
+      {
+        tag: "mcw_tfc_aio:pine_log_roofs"
+      }
+      {
+        tag: "tfc:saws"
+      }
+    ]
+    result: {
+      item: "tfc:wood/log/pine"
+      count: 1
+    }
+  }
+}

```


</details>

<details>
<summary>mcw_tfc_aio/roofs/pine_roofs/pine_plank_roof_uncraft</summary>

```diff
+{
+  type: "tfc:damage_inputs_shapeless_crafting"
+  recipe: {
+    type: "minecraft:crafting_shapeless"
+    ingredients: [
+      {
+        tag: "mcw_tfc_aio:pine_planks_roofs"
+      }
+      {
+        tag: "tfc:saws"
+      }
+    ]
+    result: {
+      item: "tfc:wood/planks/pine"
+      count: 1
+    }
+  }
+}

```


</details>

<details>
<summary>mcw_tfc_aio/roofs/pink_concrete_roofs/pink_concrete_roof_uncraft</summary>

```diff
+{
+  type: "tfc:damage_inputs_shapeless_crafting"
+  recipe: {
+    type: "minecraft:crafting_shapeless"
+    ingredients: [
+      {
+        tag: "mcw_tfc_aio:pink_concrete_roofs"
+      }
+      {
+        tag: "tfc:saws"
+      }
+    ]
+    result: {
+      item: "minecraft:pink_concrete"
+      count: 1
+    }
+  }
+}

```


</details>

<details>
<summary>mcw_tfc_aio/roofs/pink_terracotta_roofs/pink_terracotta_roof_uncraft</summary>

```diff
+{
+  type: "tfc:damage_inputs_shapeless_crafting"
+  recipe: {
+    type: "minecraft:crafting_shapeless"
+    ingredients: [
+      {
+        tag: "mcw_tfc_aio:pink_terracotta_roofs"
+      }
+      {
+        tag: "tfc:saws"
+      }
+    ]
+    result: {
+      item: "minecraft:pink_terracotta"
+      count: 1
+    }
+  }
+}

```


</details>

<details>
<summary>mcw_tfc_aio/roofs/purple_concrete_roofs/purple_concrete_roof_uncraft</summary>

```diff
+{
+  type: "tfc:damage_inputs_shapeless_crafting"
+  recipe: {
+    type: "minecraft:crafting_shapeless"
+    ingredients: [
+      {
+        tag: "mcw_tfc_aio:purple_concrete_roofs"
+      }
+      {
+        tag: "tfc:saws"
+      }
+    ]
+    result: {
+      item: "minecraft:purple_concrete"
+      count: 1
+    }
+  }
+}

```


</details>

<details>
<summary>mcw_tfc_aio/roofs/purple_terracotta_roofs/purple_terracotta_roof_uncraft</summary>

```diff
+{
+  type: "tfc:damage_inputs_shapeless_crafting"
+  recipe: {
+    type: "minecraft:crafting_shapeless"
+    ingredients: [
+      {
+        tag: "mcw_tfc_aio:purple_terracotta_roofs"
+      }
+      {
+        tag: "tfc:saws"
+      }
+    ]
+    result: {
+      item: "minecraft:purple_terracotta"
+      count: 1
+    }
+  }
+}

```


</details>

<details>
<summary>mcw_tfc_aio/roofs/red_concrete_roofs/red_concrete_roof_uncraft</summary>

```diff
+{
+  type: "tfc:damage_inputs_shapeless_crafting"
+  recipe: {
+    type: "minecraft:crafting_shapeless"
+    ingredients: [
+      {
+        tag: "mcw_tfc_aio:red_concrete_roofs"
+      }
+      {
+        tag: "tfc:saws"
+      }
+    ]
+    result: {
+      item: "minecraft:red_concrete"
+      count: 1
+    }
+  }
+}

```


</details>

<details>
<summary>mcw_tfc_aio/roofs/red_terracotta_roofs/red_terracotta_roof_uncraft</summary>

```diff
+{
+  type: "tfc:damage_inputs_shapeless_crafting"
+  recipe: {
+    type: "minecraft:crafting_shapeless"
+    ingredients: [
+      {
+        tag: "mcw_tfc_aio:red_terracotta_roofs"
+      }
+      {
+        tag: "tfc:saws"
+      }
+    ]
+    result: {
+      item: "minecraft:red_terracotta"
+      count: 1
+    }
+  }
+}

```


</details>

<details>
<summary>mcw_tfc_aio/roofs/rosewood_roofs/rosewood_log_roof_uncraft</summary>

```diff
+{
+  type: "tfc:damage_inputs_shapeless_crafting"
+  recipe: {
+    type: "minecraft:crafting_shapeless"
+    ingredients: [
+      {
+        tag: "mcw_tfc_aio:rosewood_log_roofs"
+      }
+      {
+        tag: "tfc:saws"
+      }
+    ]
+    result: {
+      item: "tfc:wood/log/rosewood"
+      count: 1
+    }
+  }
+}

```


</details>

<details>
<summary>mcw_tfc_aio/roofs/rosewood_roofs/rosewood_plank_roof_uncraft</summary>

```diff
+{
+  type: "tfc:damage_inputs_shapeless_crafting"
+  recipe: {
+    type: "minecraft:crafting_shapeless"
+    ingredients: [
+      {
+        tag: "mcw_tfc_aio:rosewood_planks_roofs"
+      }
+      {
+        tag: "tfc:saws"
+      }
+    ]
+    result: {
+      item: "tfc:wood/planks/rosewood"
+      count: 1
+    }
+  }
+}

```


</details>

<details>
<summary>mcw_tfc_aio/roofs/sequoia_roofs/sequoia_log_roof_uncraft</summary>

```diff
+{
+  type: "tfc:damage_inputs_shapeless_crafting"
+  recipe: {
+    type: "minecraft:crafting_shapeless"
+    ingredients: [
+      {
+        tag: "mcw_tfc_aio:sequoia_log_roofs"
+      }
+      {
+        tag: "tfc:saws"
+      }
+    ]
+    result: {
+      item: "tfc:wood/log/sequoia"
+      count: 1
+    }
+  }
+}

```


</details>

<details>
<summary>mcw_tfc_aio/roofs/sequoia_roofs/sequoia_plank_roof_uncraft</summary>

```diff
+{
+  type: "tfc:damage_inputs_shapeless_crafting"
+  recipe: {
+    type: "minecraft:crafting_shapeless"
+    ingredients: [
+      {
+        tag: "mcw_tfc_aio:sequoia_planks_roofs"
+      }
+      {
+        tag: "tfc:saws"
+      }
+    ]
+    result: {
+      item: "tfc:wood/planks/sequoia"
+      count: 1
+    }
+  }
+}

```


</details>

<details>
<summary>mcw_tfc_aio/roofs/spruce_roofs/spruce_log_roof_uncraft</summary>

```diff
+{
+  type: "tfc:damage_inputs_shapeless_crafting"
+  recipe: {
+    type: "minecraft:crafting_shapeless"
+    ingredients: [
+      {
+        tag: "mcw_tfc_aio:spruce_log_roofs"
+      }
+      {
+        tag: "tfc:saws"
+      }
+    ]
+    result: {
+      item: "tfc:wood/log/spruce"
+      count: 1
+    }
+  }
+}

```


</details>

<details>
<summary>mcw_tfc_aio/roofs/spruce_roofs/spruce_plank_roof_uncraft</summary>

```diff
+{
+  type: "tfc:damage_inputs_shapeless_crafting"
+  recipe: {
+    type: "minecraft:crafting_shapeless"
+    ingredients: [
+      {
+        tag: "mcw_tfc_aio:spruce_planks_roofs"
+      }
+      {
+        tag: "tfc:saws"
+      }
+    ]
+    result: {
+      item: "tfc:wood/planks/spruce"
+      count: 1
+    }
+  }
+}

```


</details>

<details>
<summary>mcw_tfc_aio/roofs/sycamore_roofs/sycamore_log_roof_uncraft</summary>

```diff
+{
+  type: "tfc:damage_inputs_shapeless_crafting"
+  recipe: {
+    type: "minecraft:crafting_shapeless"
+    ingredients: [
+      {
+        tag: "mcw_tfc_aio:sycamore_log_roofs"
+      }
+      {
+        tag: "tfc:saws"
+      }
+    ]
+    result: {
+      item: "tfc:wood/log/sycamore"
+      count: 1
+    }
+  }
+}

```


</details>

<details>
<summary>mcw_tfc_aio/roofs/sycamore_roofs/sycamore_plank_roof_uncraft</summary>

```diff
+{
+  type: "tfc:damage_inputs_shapeless_crafting"
+  recipe: {
+    type: "minecraft:crafting_shapeless"
+    ingredients: [
+      {
+        tag: "mcw_tfc_aio:sycamore_planks_roofs"
+      }
+      {
+        tag: "tfc:saws"
+      }
+    ]
+    result: {
+      item: "tfc:wood/planks/sycamore"
+      count: 1
+    }
+  }
+}

```


</details>

<details>
<summary>mcw_tfc_aio/roofs/thatch2_roofs/thatch2_attic_roof</summary>

```diff
+{
+  type: "minecraft:crafting_shaped"
+  group: "attic"
+  pattern: [
+    " W"
+    "WG"
+  ]
+  key: {
+    W: {
+      item: "tfc:thatch"
+    }
+    G: {
+      item: "minecraft:glass"
+    }
+  }
+  result: {
+    item: "mcw_tfc_aio:roofs/thatch2_roofs/thatch2_attic_roof"
+    count: 2
+  }
+}

```


</details>

<details>
<summary>mcw_tfc_aio/roofs/thatch2_roofs/thatch2_lower_roof</summary>

```diff
+{
+  type: "minecraft:crafting_shaped"
+  group: "lower"
+  pattern: [
+    " WW"
+    "WWS"
+  ]
+  key: {
+    W: {
+      item: "tfc:thatch"
+    }
+    S: {
+      item: "minecraft:stick"
+    }
+  }
+  result: {
+    item: "mcw_tfc_aio:roofs/thatch2_roofs/thatch2_lower_roof"
+    count: 4
+  }
+}

```


</details>

<details>
<summary>mcw_tfc_aio/roofs/thatch2_roofs/thatch2_roof</summary>

```diff
+{
+  type: "minecraft:crafting_shaped"
+  group: "roof"
+  pattern: [
+    " W"
+    "WS"
+  ]
+  key: {
+    W: {
+      item: "tfc:thatch"
+    }
+    S: {
+      item: "minecraft:stick"
+    }
+  }
+  result: {
+    item: "mcw_tfc_aio:roofs/thatch2_roofs/thatch2_roof"
+    count: 2
+  }
+}

```


</details>

<details>
<summary>mcw_tfc_aio/roofs/thatch2_roofs/thatch2_roof_uncraft</summary>

```diff
+{
+  type: "tfc:damage_inputs_shapeless_crafting"
+  recipe: {
+    type: "minecraft:crafting_shapeless"
+    ingredients: [
+      {
+        tag: "mcw_tfc_aio:thatch2_roofs"
+      }
+      {
+        tag: "tfc:saws"
+      }
+    ]
+    result: {
+      item: "tfc:thatch"
+      count: 1
+    }
+  }
+}

```


</details>

<details>
<summary>mcw_tfc_aio/roofs/thatch2_roofs/thatch2_steep_roof</summary>

```diff
+{
+  type: "minecraft:crafting_shaped"
+  group: "steep"
+  pattern: [
+    " W"
+    "WW"
+    "WS"
+  ]
+  key: {
+    W: {
+      item: "tfc:thatch"
+    }
+    S: {
+      item: "minecraft:stick"
+    }
+  }
+  result: {
+    item: "mcw_tfc_aio:roofs/thatch2_roofs/thatch2_steep_roof"
+    count: 4
+  }
+}

```


</details>

<details>
<summary>mcw_tfc_aio/roofs/thatch2_roofs/thatch2_top_roof</summary>

```diff
+{
+  type: "minecraft:crafting_shaped"
+  group: "top"
+  pattern: [
+    "WSW"
+  ]
+  key: {
+    W: {
+      item: "tfc:thatch"
+    }
+    S: {
+      item: "minecraft:stick"
+    }
+  }
+  result: {
+    item: "mcw_tfc_aio:roofs/thatch2_roofs/thatch2_top_roof"
+    count: 2
+  }
+}

```


</details>

<details>
<summary>mcw_tfc_aio/roofs/thatch2_roofs/thatch2_upper_lower_roof</summary>

```diff
+{
+  type: "minecraft:crafting_shaped"
+  group: "upper_lower"
+  pattern: [
+    "  W"
+    "WWS"
+  ]
+  key: {
+    W: {
+      item: "tfc:thatch"
+    }
+    S: {
+      item: "minecraft:stick"
+    }
+  }
+  result: {
+    item: "mcw_tfc_aio:roofs/thatch2_roofs/thatch2_upper_lower_roof"
+    count: 3
+  }
+}

```


</details>

<details>
<summary>mcw_tfc_aio/roofs/thatch2_roofs/thatch2_upper_steep_roof</summary>

```diff
+{
+  type: "minecraft:crafting_shaped"
+  group: "upper_steep"
+  pattern: [
+    " W"
+    " W"
+    "WS"
+  ]
+  key: {
+    W: {
+      item: "tfc:thatch"
+    }
+    S: {
+      item: "minecraft:stick"
+    }
+  }
+  result: {
+    item: "mcw_tfc_aio:roofs/thatch2_roofs/thatch2_upper_steep_roof"
+    count: 3
+  }
+}

```


</details>

<details>
<summary>mcw_tfc_aio/roofs/thatch_roofs/thatch_roof_uncraft</summary>

```diff
+{
+  type: "tfc:damage_inputs_shapeless_crafting"
+  recipe: {
+    type: "minecraft:crafting_shapeless"
+    ingredients: [
+      {
+        tag: "mcw_tfc_aio:thatch_roofs"
+      }
+      {
+        tag: "tfc:saws"
+      }
+    ]
+    result: {
+      item: "minecraft:hay_block"
+      count: 1
+    }
+  }
+}

```


</details>

<details>
<summary>mcw_tfc_aio/roofs/white_cedar_roofs/white_cedar_log_roof_uncraft</summary>

```diff
+{
+  type: "tfc:damage_inputs_shapeless_crafting"
+  recipe: {
+    type: "minecraft:crafting_shapeless"
+    ingredients: [
+      {
+        tag: "mcw_tfc_aio:white_cedar_log_roofs"
+      }
+      {
+        tag: "tfc:saws"
+      }
+    ]
+    result: {
+      item: "tfc:wood/log/white_cedar"
+      count: 1
+    }
+  }
+}

```


</details>

<details>
<summary>mcw_tfc_aio/roofs/white_cedar_roofs/white_cedar_plank_roof_uncraft</summary>

```diff
+{
+  type: "tfc:damage_inputs_shapeless_crafting"
+  recipe: {
+    type: "minecraft:crafting_shapeless"
+    ingredients: [
+      {
+        tag: "mcw_tfc_aio:white_cedar_planks_roofs"
+      }
+      {
+        tag: "tfc:saws"
+      }
+    ]
+    result: {
+      item: "tfc:wood/planks/white_cedar"
+      count: 1
+    }
+  }
+}

```


</details>

<details>
<summary>mcw_tfc_aio/roofs/white_concrete_roofs/white_concrete_roof_uncraft</summary>

```diff
+{
+  type: "tfc:damage_inputs_shapeless_crafting"
+  recipe: {
+    type: "minecraft:crafting_shapeless"
+    ingredients: [
+      {
+        tag: "mcw_tfc_aio:white_concrete_roofs"
+      }
+      {
+        tag: "tfc:saws"
+      }
+    ]
+    result: {
+      item: "minecraft:white_concrete"
+      count: 1
+    }
+  }
+}

```


</details>

<details>
<summary>mcw_tfc_aio/roofs/white_roofs/white_roof_uncraft</summary>

```diff
+{
+  type: "tfc:damage_inputs_shapeless_crafting"
+  recipe: {
+    type: "minecraft:crafting_shapeless"
+    ingredients: [
+      {
+        tag: "mcw_tfc_aio:white_roofs"
+      }
+      {
+        tag: "tfc:saws"
+      }
+    ]
+    result: {
+      item: "minecraft:white_terracotta"
+      count: 1
+    }
+  }
+}

```


</details>

<details>
<summary>mcw_tfc_aio/roofs/white_terracotta_roofs/white_terracotta_roof_uncraft</summary>

```diff
+{
+  type: "tfc:damage_inputs_shapeless_crafting"
+  recipe: {
+    type: "minecraft:crafting_shapeless"
+    ingredients: [
+      {
+        tag: "mcw_tfc_aio:white_terracotta_roofs"
+      }
+      {
+        tag: "tfc:saws"
+      }
+    ]
+    result: {
+      item: "minecraft:white_terracotta"
+      count: 1
+    }
+  }
+}

```


</details>

<details>
<summary>mcw_tfc_aio/roofs/willow_roofs/willow_log_roof_uncraft</summary>

```diff
+{
+  type: "tfc:damage_inputs_shapeless_crafting"
+  recipe: {
+    type: "minecraft:crafting_shapeless"
+    ingredients: [
+      {
+        tag: "mcw_tfc_aio:willow_log_roofs"
+      }
+      {
+        tag: "tfc:saws"
+      }
+    ]
+    result: {
+      item: "tfc:wood/log/willow"
+      count: 1
+    }
+  }
+}

```


</details>

<details>
<summary>mcw_tfc_aio/roofs/willow_roofs/willow_plank_roof_uncraft</summary>

```diff
+{
+  type: "tfc:damage_inputs_shapeless_crafting"
+  recipe: {
+    type: "minecraft:crafting_shapeless"
+    ingredients: [
+      {
+        tag: "mcw_tfc_aio:willow_planks_roofs"
+      }
+      {
+        tag: "tfc:saws"
+      }
+    ]
+    result: {
+      item: "tfc:wood/planks/willow"
+      count: 1
+    }
+  }
+}

```


</details>

<details>
<summary>mcw_tfc_aio/roofs/yellow_concrete_roofs/yellow_concrete_roof_uncraft</summary>

```diff
+{
+  type: "tfc:damage_inputs_shapeless_crafting"
+  recipe: {
+    type: "minecraft:crafting_shapeless"
+    ingredients: [
+      {
+        tag: "mcw_tfc_aio:yellow_concrete_roofs"
+      }
+      {
+        tag: "tfc:saws"
+      }
+    ]
+    result: {
+      item: "minecraft:yellow_concrete"
+      count: 1
+    }
+  }
+}

```


</details>

<details>
<summary>mcw_tfc_aio/roofs/yellow_terracotta_roofs/yellow_terracotta_roof_uncraft</summary>

```diff
+{
+  type: "tfc:damage_inputs_shapeless_crafting"
+  recipe: {
+    type: "minecraft:crafting_shapeless"
+    ingredients: [
+      {
+        tag: "mcw_tfc_aio:yellow_terracotta_roofs"
+      }
+      {
+        tag: "tfc:saws"
+      }
+    ]
+    result: {
+      item: "minecraft:yellow_terracotta"
+      count: 1
+    }
+  }
+}

```


</details>

<details>
<summary>mcw_tfc_aio/steam_boiler/roofs/thatch2_roofs/thatch2_attic_roof</summary>

```diff
+{
+  type: "gtceu:steam_boiler"
+  duration: 3600
+  inputs: {
+    item: [
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 1
+          ingredient: {
+            item: "mcw_tfc_aio:roofs/thatch2_roofs/thatch2_attic_roof"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+    ]
+  }
+  outputs: {
+  }
+  tickInputs: {
+  }
+  tickOutputs: {
+  }
+}

```


</details>

<details>
<summary>mcw_tfc_aio/steam_boiler/roofs/thatch2_roofs/thatch2_lower_roof</summary>

```diff
+{
+  type: "gtceu:steam_boiler"
+  duration: 3600
+  inputs: {
+    item: [
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 1
+          ingredient: {
+            item: "mcw_tfc_aio:roofs/thatch2_roofs/thatch2_lower_roof"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+    ]
+  }
+  outputs: {
+  }
+  tickInputs: {
+  }
+  tickOutputs: {
+  }
+}

```


</details>

<details>
<summary>mcw_tfc_aio/steam_boiler/roofs/thatch2_roofs/thatch2_roof</summary>

```diff
+{
+  type: "gtceu:steam_boiler"
+  duration: 3600
+  inputs: {
+    item: [
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 1
+          ingredient: {
+            item: "mcw_tfc_aio:roofs/thatch2_roofs/thatch2_roof"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+    ]
+  }
+  outputs: {
+  }
+  tickInputs: {
+  }
+  tickOutputs: {
+  }
+}

```


</details>

<details>
<summary>mcw_tfc_aio/steam_boiler/roofs/thatch2_roofs/thatch2_steep_roof</summary>

```diff
+{
+  type: "gtceu:steam_boiler"
+  duration: 3600
+  inputs: {
+    item: [
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 1
+          ingredient: {
+            item: "mcw_tfc_aio:roofs/thatch2_roofs/thatch2_steep_roof"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+    ]
+  }
+  outputs: {
+  }
+  tickInputs: {
+  }
+  tickOutputs: {
+  }
+}

```


</details>

<details>
<summary>mcw_tfc_aio/steam_boiler/roofs/thatch2_roofs/thatch2_top_roof</summary>

```diff
+{
+  type: "gtceu:steam_boiler"
+  duration: 3600
+  inputs: {
+    item: [
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 1
+          ingredient: {
+            item: "mcw_tfc_aio:roofs/thatch2_roofs/thatch2_top_roof"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+    ]
+  }
+  outputs: {
+  }
+  tickInputs: {
+  }
+  tickOutputs: {
+  }
+}

```


</details>

<details>
<summary>mcw_tfc_aio/steam_boiler/roofs/thatch2_roofs/thatch2_upper_lower_roof</summary>

```diff
+{
+  type: "gtceu:steam_boiler"
+  duration: 3600
+  inputs: {
+    item: [
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 1
+          ingredient: {
+            item: "mcw_tfc_aio:roofs/thatch2_roofs/thatch2_upper_lower_roof"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+    ]
+  }
+  outputs: {
+  }
+  tickInputs: {
+  }
+  tickOutputs: {
+  }
+}

```


</details>

<details>
<summary>mcw_tfc_aio/steam_boiler/roofs/thatch2_roofs/thatch2_upper_steep_roof</summary>

```diff
+{
+  type: "gtceu:steam_boiler"
+  duration: 3600
+  inputs: {
+    item: [
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 1
+          ingredient: {
+            item: "mcw_tfc_aio:roofs/thatch2_roofs/thatch2_upper_steep_roof"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+    ]
+  }
+  outputs: {
+  }
+  tickInputs: {
+  }
+  tickOutputs: {
+  }
+}

```


</details>

<details>
<summary>vintageimprovements/coiling/netherite_rod</summary>

```diff
+{
+  type: "vintageimprovements:coiling"
+  ingredients: [
+    {
+      tag: "forge:rods/netherite"
+    }
+  ]
+  results: [
+    {
+      item: "vintageimprovements:netherite_spring"
+      count: 1
+    }
+  ]
+  processingTime: 120
+  conditions: [
+    {
+      type: "forge:mod_loaded"
+      modid: "createaddition"
+    }
+  ]
+}

```


</details>

<details>
<summary>vintageimprovements/hammering/auto_smithing</summary>

```diff
+{
+  type: "vintageimprovements:auto_smithing"
+  ingredients: [
+    {
+      tag: "minecraft:trim_templates"
+    }
+    {
+      tag: "minecraft:trimmable_armor"
+    }
+    {
+      tag: "minecraft:trim_materials"
+    }
+  ]
+  results: [
+  ]
+}

```


</details>

<details>
<summary>vintageimprovements/hammering/auto_upgrade</summary>

```diff
+{
+  type: "vintageimprovements:auto_upgrade"
+  ingredients: [
+    {
+      tag: "forge:ingots/netherite"
+    }
+    [
+      {
+        item: "minecraft:diamond_helmet"
+      }
+      {
+        item: "minecraft:diamond_chestplate"
+      }
+      {
+        item: "minecraft:diamond_leggings"
+      }
+      {
+        item: "minecraft:diamond_boots"
+      }
+      {
+        item: "minecraft:diamond_sword"
+      }
+      {
+        item: "minecraft:diamond_pickaxe"
+      }
+      {
+        item: "minecraft:diamond_axe"
+      }
+      {
+        item: "minecraft:diamond_shovel"
+      }
+      {
+        item: "minecraft:diamond_hoe"
+      }
+    ]
+  ]
+  results: [
+  ]
+}

```


</details>

<details>
<summary>vintageimprovements/hammering/netherite_ingot</summary>

```diff
+{
+  type: "vintageimprovements:hammering"
+  hammerBlows: 3
+  ingredients: [
+    {
+      tag: "forge:ingots/netherite"
+    }
+  ]
+  results: [
+    {
+      item: "vintageimprovements:netherite_sheet"
+    }
+  ]
+}

```


</details>

<details>
<summary>vintageimprovements/mechanical_crafting/helve_hammer</summary>

```diff
+{
+  type: "create:mechanical_crafting"
+  acceptMirrored: true
+  key: {
+    B: {
+      tag: "forge:storage_blocks/iron"
+    }
+    L: {
+      tag: "minecraft:logs"
+    }
+    S: {
+      tag: "vintageimprovements:springs/iron"
+    }
+    C: {
+      item: "create:andesite_casing"
+    }
+    s: {
+      item: "create:shaft"
+    }
+  }
+  pattern: [
+    " B SS"
+    "BLLLC"
+    "BB  s"
+  ]
+  result: {
+    count: 1
+    item: "vintageimprovements:helve_hammer"
+  }
+}

```


</details>

<details>
<summary>vintageimprovements/rolling/netherite_plate</summary>

```diff
+{
+  type: "createaddition:rolling"
+  input: {
+    tag: "forge:plates/netherite"
+  }
+  result: {
+    item: "vintageimprovements:netherite_rod"
+    count: 2
+  }
+  conditions: [
+    {
+      type: "forge:mod_loaded"
+      modid: "createaddition"
+    }
+  ]
+}

```


</details>

</blockquote>

</details>

<details>
<summary>Changed (681)</summary>
<blockquote>

<details>
<summary>ae2/inscriber/calculation_processor_press</summary>

```diff
 {
   type: "ae2:inscriber"
   ingredients: {
     middle: {
-      item: "minecraft:iron_block"
+      tag: "forge:storage_blocks/iron"
     }
     top: {
       item: "ae2:calculation_processor_press"
     }
   }
   mode: "inscribe"
   result: {
     item: "ae2:calculation_processor_press"
   }
 }

```


</details>

<details>
<summary>ae2/inscriber/engineering_processor_press</summary>

```diff
 {
   type: "ae2:inscriber"
   ingredients: {
     middle: {
-      item: "minecraft:iron_block"
+      tag: "forge:storage_blocks/iron"
     }
     top: {
       item: "ae2:engineering_processor_press"
     }
   }
   mode: "inscribe"
   result: {
     item: "ae2:engineering_processor_press"
   }
 }

```


</details>

<details>
<summary>ae2/inscriber/logic_processor_press</summary>

```diff
 {
   type: "ae2:inscriber"
   ingredients: {
     middle: {
-      item: "minecraft:iron_block"
+      tag: "forge:storage_blocks/iron"
     }
     top: {
       item: "ae2:logic_processor_press"
     }
   }
   mode: "inscribe"
   result: {
     item: "ae2:logic_processor_press"
   }
 }

```


</details>

<details>
<summary>ae2/inscriber/silicon_press</summary>

```diff
 {
   type: "ae2:inscriber"
   ingredients: {
     middle: {
-      item: "minecraft:iron_block"
+      tag: "forge:storage_blocks/iron"
     }
     top: {
       item: "ae2:silicon_press"
     }
   }
   mode: "inscribe"
   result: {
     item: "ae2:silicon_press"
   }
 }

```


</details>

<details>
<summary>allthetweaks/atm_star_block</summary>

```diff
 {
+  category: "misc"
+  show_notification: true
   type: "minecraft:crafting_shaped"
   group: "allthetweaks"
   pattern: [
     "aaa"
     "aaa"
     "aaa"
   ]
   key: {
     a: {
       tag: "allthetweaks:atm_star"
     }
   }
   result: {
     item: "allthetweaks:atm_star_block"
   }
 }

```


</details>

<details>
<summary>allthetweaks/atm_star_from_atmstar_block</summary>

```diff
 {
+  category: "misc"
   type: "minecraft:crafting_shapeless"
   ingredients: [
     {
       tag: "forge:storage_blocks/atm_star"
     }
   ]
   result: {
     item: "allthetweaks:atm_star"
     count: 9
   }
 }

```


</details>

<details>
<summary>allthetweaks/ender_pearl_block</summary>

```diff
 {
+  category: "misc"
+  show_notification: true
   type: "minecraft:crafting_shaped"
   group: "allthetweaks"
   pattern: [
     "ppp"
     "ppp"
     "ppp"
   ]
   key: {
     p: {
       tag: "forge:ender_pearls"
     }
   }
   result: {
     item: "allthetweaks:ender_pearl_block"
   }
 }

```


</details>

<details>
<summary>allthetweaks/ender_pearl_from_ender_pearl_block</summary>

```diff
 {
+  category: "misc"
   type: "minecraft:crafting_shapeless"
   ingredients: [
     {
       tag: "forge:storage_blocks/ender_pearl"
     }
   ]
   result: {
     item: "minecraft:ender_pearl"
     count: 9
   }
 }

```


</details>

<details>
<summary>allthetweaks/nether_star_block</summary>

```diff
 {
+  category: "misc"
+  show_notification: true
   type: "minecraft:crafting_shaped"
   group: "allthetweaks"
   pattern: [
     "sss"
     "sss"
     "sss"
   ]
   key: {
     s: {
       tag: "forge:nether_stars"
     }
   }
   result: {
     item: "allthetweaks:nether_star_block"
   }
 }

```


</details>

<details>
<summary>allthetweaks/nether_star_from_nether_star_block</summary>

```diff
 {
+  category: "misc"
   type: "minecraft:crafting_shapeless"
   ingredients: [
     {
       tag: "forge:storage_blocks/nether_star"
     }
   ]
   result: {
     item: "minecraft:nether_star"
     count: 9
   }
 }

```


</details>

<details>
<summary>almostunified/ae2</summary>

```diff
 {
   type: "almostunified:client_recipe_tracker"
   namespace: "ae2"
   recipes: [
     "1$decorative/light_detector"
     "1$decorative/quartz_fixture"
+    "1$inscriber/calculation_processor_press"
+    "1$inscriber/engineering_processor_press"
+    "1$inscriber/logic_processor_press"
+    "1$inscriber/silicon_press"
   ]
 }

```


</details>

<details>
<summary>almostunified/gtceu</summary>

```diff
 {
   type: "almostunified:client_recipe_tracker"
   namespace: "gtceu"
   recipes: [
     "1$alloy_smelter/alloy_smelt_chromium_nugget_to_ingot"
     "1$alloy_smelter/alloy_smelt_chromium_to_ingot"
     "1$alloy_smelter/alloy_smelt_copper_nugget_to_ingot"
     "1$alloy_smelter/alloy_smelt_copper_to_ingot"
     "1$alloy_smelter/alloy_smelt_gold_nugget_to_ingot"
     "1$alloy_smelter/alloy_smelt_gold_to_ingot"
     "1$alloy_smelter/alloy_smelt_stainless_steel_nugget_to_ingot"
     "1$alloy_smelter/alloy_smelt_stainless_steel_to_ingot"
     "1$arc_furnace/arc_auto_maintenance_hatch"
     "1$arc_furnace/arc_brass_gear"
     "1$arc_furnace/arc_chromium_block"
     "1$arc_furnace/arc_chromium_huge_fluid_pipe"
     "1$arc_furnace/arc_chromium_large_fluid_pipe"
     "1$arc_furnace/arc_chromium_normal_fluid_pipe"
     "1$arc_furnace/arc_chromium_plate"
     "1$arc_furnace/arc_chromium_quadruple_fluid_pipe"
     "1$arc_furnace/arc_chromium_rotor"
     "1$arc_furnace/arc_chromium_small_fluid_pipe"
     "1$arc_furnace/arc_chromium_turbine_blade"
     "1$arc_furnace/arc_clean_machine_casing"
     "1$arc_furnace/arc_cleaning_maintenance_hatch"
     "1$arc_furnace/arc_cleanroom"
     "1$arc_furnace/arc_clock"
     "1$arc_furnace/arc_configurable_maintenance_hatch"
     "1$arc_furnace/arc_copper_gear"
     "1$arc_furnace/arc_cracker"
     "1$arc_furnace/arc_distillation_tower"
     "1$arc_furnace/arc_double_chromium_plate"
     "1$arc_furnace/arc_double_gold_plate"
     "1$arc_furnace/arc_double_stainless_steel_plate"
     "1$arc_furnace/arc_electrum_gear"
     "1$arc_furnace/arc_ev_chemical_reactor"
     "1$arc_furnace/arc_ev_fluid_heater"
     "1$arc_furnace/arc_ev_fluid_solidifier"
     "1$arc_furnace/arc_ev_gas_collector"
     "1$arc_furnace/arc_ev_hermetic_casing"
     "1$arc_furnace/arc_ev_mixer"
     "1$arc_furnace/arc_ev_muffler_hatch"
     "1$arc_furnace/arc_ev_ore_washer"
     "1$arc_furnace/arc_ev_pump"
     "1$arc_furnace/arc_ev_stainless_steel_drill"
     "1$arc_furnace/arc_gas_large_turbine"
     "1$arc_furnace/arc_gold_block"
     "1$arc_furnace/arc_gold_double_cable"
     "1$arc_furnace/arc_gold_double_wire"
     "1$arc_furnace/arc_gold_drum"
     "1$arc_furnace/arc_gold_dust"
     "1$arc_furnace/arc_gold_gear"
     "1$arc_furnace/arc_gold_hex_cable"
     "1$arc_furnace/arc_gold_hex_wire"
     "1$arc_furnace/arc_gold_huge_fluid_pipe"
     "1$arc_furnace/arc_gold_large_fluid_pipe"
     "1$arc_furnace/arc_gold_normal_fluid_pipe"
     "1$arc_furnace/arc_gold_octal_cable"
     "1$arc_furnace/arc_gold_octal_wire"
     "1$arc_furnace/arc_gold_plate"
     "1$arc_furnace/arc_gold_quadruple_cable"
     "1$arc_furnace/arc_gold_quadruple_fluid_pipe"
     "1$arc_furnace/arc_gold_quadruple_wire"
     "1$arc_furnace/arc_gold_small_fluid_pipe"
     "1$arc_furnace/arc_gold_spring"
     "1$arc_furnace/arc_golden_apple"
     "1$arc_furnace/arc_golden_axe"
     "1$arc_furnace/arc_golden_boots"
     "1$arc_furnace/arc_golden_chestplate"
     "1$arc_furnace/arc_golden_helmet"
     "1$arc_furnace/arc_golden_hoe"
     "1$arc_furnace/arc_golden_horse_armor"
     "1$arc_furnace/arc_golden_leggings"
     "1$arc_furnace/arc_golden_pickaxe"
     "1$arc_furnace/arc_golden_shovel"
     "1$arc_furnace/arc_golden_sword"
     "1$arc_furnace/arc_hv_16a_energy_converter"
     "1$arc_furnace/arc_hv_1a_energy_converter"
     "1$arc_furnace/arc_hv_4a_energy_converter"
     "1$arc_furnace/arc_hv_8a_energy_converter"
     "1$arc_furnace/arc_hv_alloy_smelter"
     "1$arc_furnace/arc_hv_arc_furnace"
     "1$arc_furnace/arc_hv_assembler"
     "1$arc_furnace/arc_hv_autoclave"
     "1$arc_furnace/arc_hv_battery_buffer_16x"
     "1$arc_furnace/arc_hv_battery_buffer_4x"
     "1$arc_furnace/arc_hv_battery_buffer_8x"
     "1$arc_furnace/arc_hv_bender"
     "1$arc_furnace/arc_hv_block_breaker"
     "1$arc_furnace/arc_hv_brewery"
     "1$arc_furnace/arc_hv_canner"
     "1$arc_furnace/arc_hv_centrifuge"
     "1$arc_furnace/arc_hv_chemical_bath"
     "1$arc_furnace/arc_hv_chemical_reactor"
     "1$arc_furnace/arc_hv_circuit_assembler"
     "1$arc_furnace/arc_hv_combustion"
     "1$arc_furnace/arc_hv_compressor"
     "1$arc_furnace/arc_hv_conveyor_module"
     "1$arc_furnace/arc_hv_cutter"
     "1$arc_furnace/arc_hv_diode"
     "1$arc_furnace/arc_hv_distillery"
     "1$arc_furnace/arc_hv_electric_furnace"
     "1$arc_furnace/arc_hv_electric_motor"
     "1$arc_furnace/arc_hv_electric_piston"
     "1$arc_furnace/arc_hv_electric_pump"
     "1$arc_furnace/arc_hv_electromagnetic_separator"
     "1$arc_furnace/arc_hv_emitter"
     "1$arc_furnace/arc_hv_energy_input_hatch"
     "1$arc_furnace/arc_hv_energy_output_hatch"
     "1$arc_furnace/arc_hv_extractor"
     "1$arc_furnace/arc_hv_fermenter"
     "1$arc_furnace/arc_hv_field_generator"
     "1$arc_furnace/arc_hv_fisher"
     "1$arc_furnace/arc_hv_fluid_heater"
     "1$arc_furnace/arc_hv_fluid_passthrough_hatch"
     "1$arc_furnace/arc_hv_fluid_solidifier"
     "1$arc_furnace/arc_hv_forge_hammer"
     "1$arc_furnace/arc_hv_forming_press"
     "1$arc_furnace/arc_hv_gas_collector"
     "1$arc_furnace/arc_hv_hermetic_casing"
     "1$arc_furnace/arc_hv_item_magnet"
     "1$arc_furnace/arc_hv_item_passthrough_hatch"
     "1$arc_furnace/arc_hv_laser_engraver"
     "1$arc_furnace/arc_hv_lathe"
     "1$arc_furnace/arc_hv_macerator"
     "1$arc_furnace/arc_hv_machine_casing"
     "1$arc_furnace/arc_hv_machine_hull"
     "1$arc_furnace/arc_hv_miner"
     "1$arc_furnace/arc_hv_mixer"
     "1$arc_furnace/arc_hv_muffler_hatch"
     "1$arc_furnace/arc_hv_ore_washer"
     "1$arc_furnace/arc_hv_packer"
     "1$arc_furnace/arc_hv_polarizer"
     "1$arc_furnace/arc_hv_pump"
     "1$arc_furnace/arc_hv_rock_crusher"
     "1$arc_furnace/arc_hv_rotor_holder"
     "1$arc_furnace/arc_hv_sensor"
     "1$arc_furnace/arc_hv_sifter"
-    "1$arc_furnace/arc_hv_stainless_steel_drill"
-    "1$arc_furnace/arc_hv_stainless_steel_wrench"
     "1$arc_furnace/arc_hv_steam_turbine"
     "1$arc_furnace/arc_hv_super_chest"
     "1$arc_furnace/arc_hv_super_tank"
     "1$arc_furnace/arc_hv_thermal_centrifuge"
     "1$arc_furnace/arc_hv_transformer_16a"
     "1$arc_furnace/arc_hv_transformer_1a"
     "1$arc_furnace/arc_hv_transformer_2a"
     "1$arc_furnace/arc_hv_transformer_4a"
     "1$arc_furnace/arc_hv_wiremill"
     "1$arc_furnace/arc_hv_world_accelerator"
     "1$arc_furnace/arc_implosion_compressor"
     "1$arc_furnace/arc_iv_processing_array"
     "1$arc_furnace/arc_iv_quantum_chest"
     "1$arc_furnace/arc_iv_stainless_steel_drill"
     "1$arc_furnace/arc_iv_stainless_steel_wrench"
     "1$arc_furnace/arc_large_centrifuge"
     "1$arc_furnace/arc_large_chemical_reactor"
     "1$arc_furnace/arc_large_distillery"
     "1$arc_furnace/arc_large_packer"
     "1$arc_furnace/arc_lead_gear"
     "1$arc_furnace/arc_light_weighted_pressure_plate"
     "1$arc_furnace/arc_long_gold_rod"
     "1$arc_furnace/arc_long_stainless_steel_rod"
     "1$arc_furnace/arc_lv_electrolyzer"
     "1$arc_furnace/arc_lv_stainless_steel_chainsaw"
     "1$arc_furnace/arc_lv_stainless_steel_drill"
     "1$arc_furnace/arc_lv_stainless_steel_screwdriver"
     "1$arc_furnace/arc_lv_stainless_steel_wrench"
     "1$arc_furnace/arc_mv_stainless_steel_drill"
     "1$arc_furnace/arc_mv_transformer_16a"
     "1$arc_furnace/arc_mv_transformer_2a"
     "1$arc_furnace/arc_mv_transformer_4a"
     "1$arc_furnace/arc_nichrome_coil_block"
     "1$arc_furnace/arc_nickel_gear"
     "1$arc_furnace/arc_osmium_gear"
     "1$arc_furnace/arc_platinum_gear"
     "1$arc_furnace/arc_prospector.hv"
     "1$arc_furnace/arc_silver_gear"
     "1$arc_furnace/arc_small_stainless_steel_gear"
     "1$arc_furnace/arc_stainless_steel_block"
     "1$arc_furnace/arc_stainless_steel_buzzsaw"
     "1$arc_furnace/arc_stainless_steel_crate"
     "1$arc_furnace/arc_stainless_steel_drum"
     "1$arc_furnace/arc_stainless_steel_fluid_cell"
     "1$arc_furnace/arc_stainless_steel_frame"
     "1$arc_furnace/arc_stainless_steel_gear"
     "1$arc_furnace/arc_stainless_steel_gearbox"
     "1$arc_furnace/arc_stainless_steel_huge_fluid_pipe"
     "1$arc_furnace/arc_stainless_steel_large_fluid_pipe"
     "1$arc_furnace/arc_stainless_steel_normal_fluid_pipe"
     "1$arc_furnace/arc_stainless_steel_plate"
     "1$arc_furnace/arc_stainless_steel_quadruple_fluid_pipe"
     "1$arc_furnace/arc_stainless_steel_rotor"
     "1$arc_furnace/arc_stainless_steel_small_fluid_pipe"
     "1$arc_furnace/arc_stainless_steel_turbine_blade"
     "1$arc_furnace/arc_stainless_steel_turbine_casing"
     "1$arc_furnace/arc_tin_gear"
     "1$arc_furnace/arc_titanium_large_boiler"
     "1$arc_furnace/arc_uranium_gear"
     "1$arc_furnace/arc_vacuum_freezer"
     "1$arc_furnace/arc_zinc_gear"
     "1$autoclave/autoclave_dust_apatite__distilled"
     "1$autoclave/autoclave_dust_apatite__water"
     "1$autoclave/autoclave_dust_cinnabar__distilled"
     "1$autoclave/autoclave_dust_cinnabar__water"
     "1$autoclave/autoclave_dust_lapis__distilled"
     "1$autoclave/autoclave_dust_lapis__water"
     "1$blasting/smelt_bornite_ore_to_ingot"
     "1$blasting/smelt_chalcocite_ore_to_ingot"
     "1$blasting/smelt_chalcopyrite_ore_to_ingot"
     "1$blasting/smelt_copper_ore_to_ingot"
     "1$blasting/smelt_deepslate_bornite_ore_to_ingot"
     "1$blasting/smelt_deepslate_chalcocite_ore_to_ingot"
     "1$blasting/smelt_deepslate_chalcopyrite_ore_to_ingot"
     "1$blasting/smelt_deepslate_copper_ore_to_ingot"
     "1$blasting/smelt_deepslate_diamond_ore_to_ingot"
     "1$blasting/smelt_deepslate_emerald_ore_to_ingot"
     "1$blasting/smelt_deepslate_gold_ore_to_ingot"
     "1$blasting/smelt_deepslate_lapis_ore_to_ingot"
     "1$blasting/smelt_deepslate_malachite_ore_to_ingot"
     "1$blasting/smelt_deepslate_tetrahedrite_ore_to_ingot"
     "1$blasting/smelt_diamond_ore_to_ingot"
     "1$blasting/smelt_emerald_ore_to_ingot"
     "1$blasting/smelt_endstone_bornite_ore_to_ingot"
     "1$blasting/smelt_endstone_chalcocite_ore_to_ingot"
     "1$blasting/smelt_endstone_chalcopyrite_ore_to_ingot"
     "1$blasting/smelt_endstone_copper_ore_to_ingot"
     "1$blasting/smelt_endstone_diamond_ore_to_ingot"
     "1$blasting/smelt_endstone_emerald_ore_to_ingot"
     "1$blasting/smelt_endstone_gold_ore_to_ingot"
     "1$blasting/smelt_endstone_lapis_ore_to_ingot"
     "1$blasting/smelt_endstone_malachite_ore_to_ingot"
     "1$blasting/smelt_endstone_tetrahedrite_ore_to_ingot"
     "1$blasting/smelt_gold_ore_to_ingot"
     "1$blasting/smelt_lapis_ore_to_ingot"
     "1$blasting/smelt_malachite_ore_to_ingot"
     "1$blasting/smelt_netherrack_bornite_ore_to_ingot"
     "1$blasting/smelt_netherrack_chalcocite_ore_to_ingot"
     "1$blasting/smelt_netherrack_chalcopyrite_ore_to_ingot"
     "1$blasting/smelt_netherrack_copper_ore_to_ingot"
     "1$blasting/smelt_netherrack_diamond_ore_to_ingot"
     "1$blasting/smelt_netherrack_emerald_ore_to_ingot"
     "1$blasting/smelt_netherrack_gold_ore_to_ingot"
     "1$blasting/smelt_netherrack_lapis_ore_to_ingot"
     "1$blasting/smelt_netherrack_malachite_ore_to_ingot"
     "1$blasting/smelt_netherrack_tetrahedrite_ore_to_ingot"
     "1$blasting/smelt_raw_bornite_ore_to_ingot"
     "1$blasting/smelt_raw_chalcocite_ore_to_ingot"
     "1$blasting/smelt_raw_chalcopyrite_ore_to_ingot"
     "1$blasting/smelt_raw_diamond_ore_to_ingot"
     "1$blasting/smelt_raw_emerald_ore_to_ingot"
     "1$blasting/smelt_raw_lapis_ore_to_ingot"
     "1$blasting/smelt_raw_malachite_ore_to_ingot"
     "1$blasting/smelt_raw_tetrahedrite_ore_to_ingot"
     "1$blasting/smelt_tetrahedrite_ore_to_ingot"
     "1$compressor/compress_chromium_nugget_to_ingot"
     "1$compressor/compress_copper_nugget_to_ingot"
     "1$compressor/compress_gold_nugget_to_ingot"
     "1$compressor/compress_plate_dust_obsidian_"
     "1$compressor/compress_stainless_steel_nugget_to_ingot"
     "1$cutter/cut_diamond_flawless_gem_to_gem"
     "1$cutter/cut_diamond_flawless_gem_to_gem_distilled_water"
     "1$cutter/cut_diamond_flawless_gem_to_gem_water"
     "1$cutter/cut_emerald_flawless_gem_to_gem"
     "1$cutter/cut_emerald_flawless_gem_to_gem_distilled_water"
     "1$cutter/cut_emerald_flawless_gem_to_gem_water"
     "1$cutter/cut_lapis_flawless_gem_to_gem"
     "1$cutter/cut_lapis_flawless_gem_to_gem_distilled_water"
     "1$cutter/cut_lapis_flawless_gem_to_gem_water"
     "1$cutter/cut_stainless_steel_long_rod_to_rod"
     "1$cutter/cut_stainless_steel_long_rod_to_rod_distilled_water"
     "1$cutter/cut_stainless_steel_long_rod_to_rod_water"
     "1$electric_blast_furnace/blast_chromium"
     "1$electric_blast_furnace/blast_chromium_gas"
     "1$electric_blast_furnace/blast_stainless_steel"
     "1$electric_blast_furnace/blast_stainless_steel_gas"
     "1$extractor/charcoal_extraction"
     "1$extruder/extrude_chromium_to_rod"
     "1$extruder/extrude_stainless_steel_to_rod"
     "1$fluid_solidifier/solidify_chromium_to_ingot"
     "1$fluid_solidifier/solidify_copper_to_ingot"
     "1$fluid_solidifier/solidify_gold_to_ingot"
     "1$fluid_solidifier/solidify_stainless_steel_to_ingot"
     "1$forge_hammer/hammer_diamond_block_to_gem"
     "1$forge_hammer/hammer_emerald_block_to_gem"
     "1$forge_hammer/hammer_lapis_block_to_gem"
     "1$implosion_compressor/implode_dust_apatite__tnt"
     "1$implosion_compressor/implode_dust_cinnabar__tnt"
     "1$implosion_compressor/implode_dust_diamond__tnt"
     "1$implosion_compressor/implode_dust_emerald__tnt"
     "1$implosion_compressor/implode_dust_fluorite__tnt"
     "1$implosion_compressor/implode_dust_lapis__tnt"
     "1$implosion_compressor/implode_dust_ruby__tnt"
     "1$implosion_compressor/implode_dust_sapphire__tnt"
     "1$large_boiler/charcoal_block"
     "1$large_boiler/charcoal_dust"
     "1$large_boiler/coal_dust"
     "1$laser_engraver/engrave_apatite_flawless_gem_to_gem"
     "1$laser_engraver/engrave_cinnabar_flawless_gem_to_gem"
     "1$laser_engraver/engrave_coal_flawless_gem_to_gem"
     "1$laser_engraver/engrave_diamond_flawless_gem_to_gem"
     "1$laser_engraver/engrave_diamond_gem_to_flawed_gem"
     "1$laser_engraver/engrave_emerald_flawless_gem_to_gem"
     "1$laser_engraver/engrave_emerald_gem_to_flawed_gem"
     "1$laser_engraver/engrave_fluorite_flawless_gem_to_gem"
     "1$laser_engraver/engrave_lapis_flawless_gem_to_gem"
     "1$laser_engraver/engrave_lapis_gem_to_flawed_gem"
     "1$laser_engraver/engrave_ruby_flawless_gem_to_gem"
     "1$laser_engraver/engrave_sapphire_flawless_gem_to_gem"
     "1$lathe/lathe_chromium_to_rod"
     "1$lathe/lathe_stainless_steel_to_rod"
     "1$macerator/macerate_beryllium_ore_to_raw_ore"
     "1$macerator/macerate_brass_gear"
     "1$macerator/macerate_copper_gear"
     "1$macerator/macerate_deepslate_beryllium_ore_to_raw_ore"
     "1$macerator/macerate_electrum_gear"
     "1$macerator/macerate_endstone_beryllium_ore_to_raw_ore"
     "1$macerator/macerate_fluorite_ingot"
     "1$macerator/macerate_fluorite_nugget"
     "1$macerator/macerate_gold_gear"
     "1$macerator/macerate_graphite_block"
     "1$macerator/macerate_graphite_ingot"
     "1$macerator/macerate_graphite_nugget"
     "1$macerator/macerate_lead_gear"
     "1$macerator/macerate_netherrack_beryllium_ore_to_raw_ore"
     "1$macerator/macerate_nickel_gear"
     "1$macerator/macerate_niob_block"
     "1$macerator/macerate_osmium_gear"
     "1$macerator/macerate_platinum_gear"
     "1$macerator/macerate_silver_gear"
     "1$macerator/macerate_sulfur"
     "1$macerator/macerate_sulfur_block"
     "1$macerator/macerate_sulfur_chunk"
     "1$macerator/macerate_tin_gear"
     "1$macerator/macerate_uranium_gear"
     "1$macerator/macerate_zinc_gear"
     "1$pyrolyse_oven/charcoal_to_coal_tar"
     "1$pyrolyse_oven/coal_to_coal_tar"
     "1$shaped/stick_chromium"
     "1$shaped/stick_long_stainless_steel"
     "1$shaped/stick_stainless_steel"
     "1$shapeless/gem_to_gem_gem_diamond"
     "1$shapeless/gem_to_gem_gem_emerald"
     "1$shapeless/gem_to_gem_gem_lapis"
     "1$sifter/sift_diamond_purified_ore_to_gems"
     "1$sifter/sift_emerald_purified_ore_to_gems"
     "1$sifter/sift_lapis_purified_ore_to_gems"
     "1$smelting/dust_bornite__dust_to_ingot"
     "1$smelting/dust_chalcocite__dust_to_ingot"
     "1$smelting/dust_chalcopyrite__dust_to_ingot"
     "1$smelting/dust_copper__demagnetize_from_dust"
     "1$smelting/dust_gold__demagnetize_from_dust"
     "1$smelting/dust_malachite__ingot"
     "1$smelting/dust_tetrahedrite__dust_to_ingot"
     "1$smelting/smelt_bornite_ore_to_ingot"
     "1$smelting/smelt_chalcocite_ore_to_ingot"
     "1$smelting/smelt_chalcopyrite_ore_to_ingot"
     "1$smelting/smelt_copper_ore_to_ingot"
     "1$smelting/smelt_crushed_ore_bornite_to_ingot"
     "1$smelting/smelt_crushed_ore_chalcocite_to_ingot"
     "1$smelting/smelt_crushed_ore_chalcopyrite_to_ingot"
     "1$smelting/smelt_crushed_ore_copper_to_ingot"
     "1$smelting/smelt_crushed_ore_gold_to_ingot"
     "1$smelting/smelt_crushed_ore_malachite_to_ingot"
     "1$smelting/smelt_crushed_ore_tetrahedrite_to_ingot"
     "1$smelting/smelt_deepslate_bornite_ore_to_ingot"
     "1$smelting/smelt_deepslate_chalcocite_ore_to_ingot"
     "1$smelting/smelt_deepslate_chalcopyrite_ore_to_ingot"
     "1$smelting/smelt_deepslate_copper_ore_to_ingot"
     "1$smelting/smelt_deepslate_diamond_ore_to_ingot"
     "1$smelting/smelt_deepslate_emerald_ore_to_ingot"
     "1$smelting/smelt_deepslate_gold_ore_to_ingot"
     "1$smelting/smelt_deepslate_lapis_ore_to_ingot"
     "1$smelting/smelt_deepslate_malachite_ore_to_ingot"
     "1$smelting/smelt_deepslate_tetrahedrite_ore_to_ingot"
     "1$smelting/smelt_diamond_ore_to_ingot"
     "1$smelting/smelt_emerald_ore_to_ingot"
     "1$smelting/smelt_endstone_bornite_ore_to_ingot"
     "1$smelting/smelt_endstone_chalcocite_ore_to_ingot"
     "1$smelting/smelt_endstone_chalcopyrite_ore_to_ingot"
     "1$smelting/smelt_endstone_copper_ore_to_ingot"
     "1$smelting/smelt_endstone_diamond_ore_to_ingot"
     "1$smelting/smelt_endstone_emerald_ore_to_ingot"
     "1$smelting/smelt_endstone_gold_ore_to_ingot"
     "1$smelting/smelt_endstone_lapis_ore_to_ingot"
     "1$smelting/smelt_endstone_malachite_ore_to_ingot"
     "1$smelting/smelt_endstone_tetrahedrite_ore_to_ingot"
     "1$smelting/smelt_gold_ore_to_ingot"
     "1$smelting/smelt_impure_dust_bornite_to_ingot"
     "1$smelting/smelt_impure_dust_chalcocite_to_ingot"
     "1$smelting/smelt_impure_dust_chalcopyrite_to_ingot"
     "1$smelting/smelt_impure_dust_copper_to_ingot"
     "1$smelting/smelt_impure_dust_gold_to_ingot"
     "1$smelting/smelt_impure_dust_malachite_to_ingot"
     "1$smelting/smelt_impure_dust_tetrahedrite_to_ingot"
     "1$smelting/smelt_lapis_ore_to_ingot"
     "1$smelting/smelt_malachite_ore_to_ingot"
     "1$smelting/smelt_netherrack_bornite_ore_to_ingot"
     "1$smelting/smelt_netherrack_chalcocite_ore_to_ingot"
     "1$smelting/smelt_netherrack_chalcopyrite_ore_to_ingot"
     "1$smelting/smelt_netherrack_copper_ore_to_ingot"
     "1$smelting/smelt_netherrack_diamond_ore_to_ingot"
     "1$smelting/smelt_netherrack_emerald_ore_to_ingot"
     "1$smelting/smelt_netherrack_gold_ore_to_ingot"
     "1$smelting/smelt_netherrack_lapis_ore_to_ingot"
     "1$smelting/smelt_netherrack_malachite_ore_to_ingot"
     "1$smelting/smelt_netherrack_tetrahedrite_ore_to_ingot"
     "1$smelting/smelt_pure_dust_bornite_to_ingot"
     "1$smelting/smelt_pure_dust_chalcocite_to_ingot"
     "1$smelting/smelt_pure_dust_chalcopyrite_to_ingot"
     "1$smelting/smelt_pure_dust_copper_to_ingot"
     "1$smelting/smelt_pure_dust_gold_to_ingot"
     "1$smelting/smelt_pure_dust_malachite_to_ingot"
     "1$smelting/smelt_pure_dust_tetrahedrite_to_ingot"
     "1$smelting/smelt_purified_ore_bornite_to_ingot"
     "1$smelting/smelt_purified_ore_chalcocite_to_ingot"
     "1$smelting/smelt_purified_ore_chalcopyrite_to_ingot"
     "1$smelting/smelt_purified_ore_copper_to_ingot"
     "1$smelting/smelt_purified_ore_gold_to_ingot"
     "1$smelting/smelt_purified_ore_malachite_to_ingot"
     "1$smelting/smelt_purified_ore_tetrahedrite_to_ingot"
     "1$smelting/smelt_raw_bornite_ore_to_ingot"
     "1$smelting/smelt_raw_chalcocite_ore_to_ingot"
     "1$smelting/smelt_raw_chalcopyrite_ore_to_ingot"
     "1$smelting/smelt_raw_diamond_ore_to_ingot"
     "1$smelting/smelt_raw_emerald_ore_to_ingot"
     "1$smelting/smelt_raw_lapis_ore_to_ingot"
     "1$smelting/smelt_raw_malachite_ore_to_ingot"
     "1$smelting/smelt_raw_tetrahedrite_ore_to_ingot"
     "1$smelting/smelt_refined_ore_bornite_to_ingot"
     "1$smelting/smelt_refined_ore_chalcocite_to_ingot"
     "1$smelting/smelt_refined_ore_chalcopyrite_to_ingot"
     "1$smelting/smelt_refined_ore_copper_to_ingot"
     "1$smelting/smelt_refined_ore_gold_to_ingot"
     "1$smelting/smelt_refined_ore_malachite_to_ingot"
     "1$smelting/smelt_refined_ore_tetrahedrite_to_ingot"
     "1$smelting/smelt_tetrahedrite_ore_to_ingot"
     "1$steam_boiler/charcoal_block"
     "1$steam_boiler/charcoal_dust"
     "1$steam_boiler/coal_dust"
   ]
 }

```


</details>

<details>
<summary>almostunified/megacells</summary>

```diff
 {
   type: "almostunified:client_recipe_tracker"
   namespace: "megacells"
   recipes: [
     "1$cells/standard/bulk_item_cell"
+    "1$inscriber/accumulation_processor_press_extra"
   ]
 }

```


</details>

<details>
<summary>almostunified/minecraft</summary>

```diff
 {
   type: "almostunified:client_recipe_tracker"
   namespace: "minecraft"
   recipes: [
     "1$aluminum_ingot_from_smelting"
     "1$aluminum_ingot_from_smelting_deepslate"
     "1$blue_dye"
     "1$chain"
-    "1$chromium_ingot_from_smelting"
-    "1$chromium_ingot_from_smelting_deeplate"
     "1$copper_block"
     "1$copper_ingot_from_blasting_raw_copper"
     "1$copper_ingot_from_smelting_raw_copper"
     "1$copper_ingot_from_waxed_copper_block"
     "1$cut_copper"
     "1$cut_copper_from_copper_block_stonecutting"
     "1$cut_copper_slab_from_copper_block_stonecutting"
     "1$cut_copper_stairs_from_copper_block_stonecutting"
     "1$fire_charge"
     "1$fluorite_ingot_from_smelting"
     "1$glistering_melon_slice"
     "1$gold_ingot_from_blasting_raw_gold"
     "1$gold_ingot_from_smelting_raw_gold"
     "1$golden_carrot"
     "1$graphite_ingot_from_smelting"
     "1$iron_ingot_from_blasting_raw_iron"
     "1$iron_ingot_from_smelting_raw_iron"
     "1$large_boiler/charcoal"
     "1$large_boiler/coal"
     "1$large_boiler/coal_block"
     "1$manganese_ingot_from_smelting"
     "1$manganese_ingot_from_smelting_deepslate"
     "1$molybdenum_ingot_from_smelting"
     "1$molybdenum_ingot_from_smelting_deepslate"
     "1$netherite_axe_smithing"
     "1$netherite_block"
     "1$netherite_boots_smithing"
     "1$netherite_chestplate_smithing"
     "1$netherite_helmet_smithing"
     "1$netherite_hoe_smithing"
     "1$netherite_ingot_from_netherite_block"
     "1$netherite_leggings_smithing"
     "1$netherite_pickaxe_smithing"
     "1$netherite_shovel_smithing"
     "1$netherite_sword_smithing"
     "1$nickel_ingot_from_smelting"
     "1$nickel_ingot_from_smelting_deepslate"
     "1$niob_ingot_from_smelting"
     "1$niob_ingot_from_smelting_deepslate"
     "1$raw_copper"
     "1$raw_copper_block"
     "1$raw_gold"
     "1$raw_gold_block"
     "1$raw_iron"
     "1$raw_iron_block"
     "1$soul_lantern"
     "1$steam_boiler/charcoal"
     "1$steam_boiler/coal"
     "1$steam_boiler/coal_block"
     "1$titanium_ingot_from_smelting"
     "1$titanium_ingot_from_smelting_deepslate"
     "1$uranium_ingot_from_smelting"
     "1$uranium_ingot_from_smelting_deepslate"
     "1$waxed_copper_block_from_honeycomb"
     "3$coal_from_blasting_coal_ore"
     "3$coal_from_blasting_deepslate_coal_ore"
     "3$coal_from_smelting_coal_ore"
     "3$coal_from_smelting_deepslate_coal_ore"
     "3$copper_ingot"
     "3$copper_ingot_from_blasting_copper_ore"
     "3$copper_ingot_from_blasting_deepslate_copper_ore"
     "3$copper_ingot_from_smelting_copper_ore"
     "3$copper_ingot_from_smelting_deepslate_copper_ore"
     "3$diamond_from_blasting_deepslate_diamond_ore"
     "3$diamond_from_blasting_diamond_ore"
     "3$diamond_from_smelting_deepslate_diamond_ore"
     "3$diamond_from_smelting_diamond_ore"
     "3$emerald_from_blasting_deepslate_emerald_ore"
     "3$emerald_from_blasting_emerald_ore"
     "3$emerald_from_smelting_deepslate_emerald_ore"
     "3$emerald_from_smelting_emerald_ore"
     "3$gold_ingot_from_blasting_deepslate_gold_ore"
     "3$gold_ingot_from_blasting_gold_ore"
     "3$gold_ingot_from_blasting_nether_gold_ore"
     "3$gold_ingot_from_smelting_deepslate_gold_ore"
     "3$gold_ingot_from_smelting_gold_ore"
     "3$gold_ingot_from_smelting_nether_gold_ore"
     "3$iron_ingot_from_blasting_deepslate_iron_ore"
     "3$iron_ingot_from_blasting_iron_ore"
     "3$iron_ingot_from_smelting_deepslate_iron_ore"
     "3$iron_ingot_from_smelting_iron_ore"
     "3$lapis_lazuli_from_blasting_deepslate_lapis_ore"
     "3$lapis_lazuli_from_blasting_lapis_ore"
     "3$lapis_lazuli_from_smelting_deepslate_lapis_ore"
     "3$lapis_lazuli_from_smelting_lapis_ore"
     "3$lead_ingot_from_blasting_deepslate_lead_ore"
     "3$lead_ingot_from_blasting_lead_ore"
     "3$lead_ingot_from_blasting_lead_raw"
     "3$lead_ingot_from_smelting_deepslate_lead_ore"
     "3$lead_ingot_from_smelting_lead_ore"
     "3$lead_ingot_from_smelting_lead_raw"
     "3$nickel_ingot_from_blasting_deepslate_nickel_ore"
     "3$nickel_ingot_from_blasting_nickel_ore"
     "3$nickel_ingot_from_blasting_nickel_raw"
     "3$nickel_ingot_from_smelting_deepslate_nickel_ore"
     "3$nickel_ingot_from_smelting_nickel_ore"
     "3$nickel_ingot_from_smelting_nickel_raw"
     "3$silver_ingot_from_blasting_deepslate_silver_ore"
     "3$silver_ingot_from_blasting_silver_ore"
     "3$silver_ingot_from_blasting_silver_raw"
     "3$silver_ingot_from_smelting_deepslate_silver_ore"
     "3$silver_ingot_from_smelting_silver_ore"
     "3$silver_ingot_from_smelting_silver_raw"
     "3$tin_ingot_from_blasting_deepslate_tin_ore"
     "3$tin_ingot_from_blasting_tin_ore"
     "3$tin_ingot_from_blasting_tin_raw"
     "3$tin_ingot_from_smelting_deepslate_tin_ore"
     "3$tin_ingot_from_smelting_tin_ore"
     "3$tin_ingot_from_smelting_tin_raw"
     "3$zinc_ingot_from_blasting_deepslate_zinc_ore"
     "3$zinc_ingot_from_blasting_zinc_ore"
     "3$zinc_ingot_from_blasting_zinc_raw"
     "3$zinc_ingot_from_smelting_deepslate_zinc_ore"
     "3$zinc_ingot_from_smelting_zinc_ore"
     "3$zinc_ingot_from_smelting_zinc_raw"
   ]
 }

```


</details>

<details>
<summary>gtceu/alloy_smelter/andesite_brick</summary>

```diff
 {
   type: "gtceu:alloy_smelter"
-  duration: 120
+  duration: 60
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "tfc:rock/loose/andesite"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "gtceu:ingot_casting_mold"
           }
         }
         chance: 0
         tierChanceBoost: 0
       }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "tfc:brick/andesite"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
 }

```


</details>

<details>
<summary>gtceu/alloy_smelter/basalt_brick</summary>

```diff
 {
   type: "gtceu:alloy_smelter"
-  duration: 120
+  duration: 60
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "tfc:rock/loose/basalt"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "gtceu:ingot_casting_mold"
           }
         }
         chance: 0
         tierChanceBoost: 0
       }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "tfc:brick/basalt"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
 }

```


</details>

<details>
<summary>gtceu/alloy_smelter/brick</summary>

```diff
 {
   type: "gtceu:alloy_smelter"
-  duration: 120
+  duration: 60
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "minecraft:clay_ball"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "gtceu:ingot_casting_mold"
           }
         }
         chance: 0
         tierChanceBoost: 0
       }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "minecraft:brick"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
 }

```


</details>

<details>
<summary>gtceu/alloy_smelter/chalk_brick</summary>

```diff
 {
   type: "gtceu:alloy_smelter"
-  duration: 120
+  duration: 60
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "tfc:rock/loose/chalk"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "gtceu:ingot_casting_mold"
           }
         }
         chance: 0
         tierChanceBoost: 0
       }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "tfc:brick/chalk"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
 }

```


</details>

<details>
<summary>gtceu/alloy_smelter/chert_brick</summary>

```diff
 {
   type: "gtceu:alloy_smelter"
-  duration: 120
+  duration: 60
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "tfc:rock/loose/chert"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "gtceu:ingot_casting_mold"
           }
         }
         chance: 0
         tierChanceBoost: 0
       }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "tfc:brick/chert"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
 }

```


</details>

<details>
<summary>gtceu/alloy_smelter/claystone_brick</summary>

```diff
 {
   type: "gtceu:alloy_smelter"
-  duration: 120
+  duration: 60
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "tfc:rock/loose/claystone"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "gtceu:ingot_casting_mold"
           }
         }
         chance: 0
         tierChanceBoost: 0
       }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "tfc:brick/claystone"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
 }

```


</details>

<details>
<summary>gtceu/alloy_smelter/conglomerate_brick</summary>

```diff
 {
   type: "gtceu:alloy_smelter"
-  duration: 120
+  duration: 60
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "tfc:rock/loose/conglomerate"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "gtceu:ingot_casting_mold"
           }
         }
         chance: 0
         tierChanceBoost: 0
       }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "tfc:brick/conglomerate"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
 }

```


</details>

<details>
<summary>gtceu/alloy_smelter/dacite_brick</summary>

```diff
 {
   type: "gtceu:alloy_smelter"
-  duration: 120
+  duration: 60
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "tfc:rock/loose/dacite"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "gtceu:ingot_casting_mold"
           }
         }
         chance: 0
         tierChanceBoost: 0
       }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "tfc:brick/dacite"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
 }

```


</details>

<details>
<summary>gtceu/alloy_smelter/diorite_brick</summary>

```diff
 {
   type: "gtceu:alloy_smelter"
-  duration: 120
+  duration: 60
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "tfc:rock/loose/diorite"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "gtceu:ingot_casting_mold"
           }
         }
         chance: 0
         tierChanceBoost: 0
       }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "tfc:brick/diorite"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
 }

```


</details>

<details>
<summary>gtceu/alloy_smelter/dolomite_brick</summary>

```diff
 {
   type: "gtceu:alloy_smelter"
-  duration: 120
+  duration: 60
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "tfc:rock/loose/dolomite"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "gtceu:ingot_casting_mold"
           }
         }
         chance: 0
         tierChanceBoost: 0
       }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "tfc:brick/dolomite"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
 }

```


</details>

<details>
<summary>gtceu/alloy_smelter/gabbro_brick</summary>

```diff
 {
   type: "gtceu:alloy_smelter"
-  duration: 120
+  duration: 60
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "tfc:rock/loose/gabbro"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "gtceu:ingot_casting_mold"
           }
         }
         chance: 0
         tierChanceBoost: 0
       }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "tfc:brick/gabbro"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
 }

```


</details>

<details>
<summary>gtceu/alloy_smelter/gneiss_brick</summary>

```diff
 {
   type: "gtceu:alloy_smelter"
-  duration: 120
+  duration: 60
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "tfc:rock/loose/gneiss"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "gtceu:ingot_casting_mold"
           }
         }
         chance: 0
         tierChanceBoost: 0
       }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "tfc:brick/gneiss"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
 }

```


</details>

<details>
<summary>gtceu/alloy_smelter/granite_brick</summary>

```diff
 {
   type: "gtceu:alloy_smelter"
-  duration: 120
+  duration: 60
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "tfc:rock/loose/granite"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "gtceu:ingot_casting_mold"
           }
         }
         chance: 0
         tierChanceBoost: 0
       }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "tfc:brick/granite"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
 }

```


</details>

<details>
<summary>gtceu/alloy_smelter/limestone_brick</summary>

```diff
 {
   type: "gtceu:alloy_smelter"
-  duration: 120
+  duration: 60
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "tfc:rock/loose/limestone"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "gtceu:ingot_casting_mold"
           }
         }
         chance: 0
         tierChanceBoost: 0
       }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "tfc:brick/limestone"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
 }

```


</details>

<details>
<summary>gtceu/alloy_smelter/marble_brick</summary>

```diff
 {
   type: "gtceu:alloy_smelter"
-  duration: 120
+  duration: 60
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "tfc:rock/loose/marble"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "gtceu:ingot_casting_mold"
           }
         }
         chance: 0
         tierChanceBoost: 0
       }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "tfc:brick/marble"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
 }

```


</details>

<details>
<summary>gtceu/alloy_smelter/phyllite_brick</summary>

```diff
 {
   type: "gtceu:alloy_smelter"
-  duration: 120
+  duration: 60
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "tfc:rock/loose/phyllite"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "gtceu:ingot_casting_mold"
           }
         }
         chance: 0
         tierChanceBoost: 0
       }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "tfc:brick/phyllite"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
 }

```


</details>

<details>
<summary>gtceu/alloy_smelter/quartzite_brick</summary>

```diff
 {
   type: "gtceu:alloy_smelter"
-  duration: 120
+  duration: 60
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "tfc:rock/loose/quartzite"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "gtceu:ingot_casting_mold"
           }
         }
         chance: 0
         tierChanceBoost: 0
       }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "tfc:brick/quartzite"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
 }

```


</details>

<details>
<summary>gtceu/alloy_smelter/rhyolite_brick</summary>

```diff
 {
   type: "gtceu:alloy_smelter"
-  duration: 120
+  duration: 60
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "tfc:rock/loose/rhyolite"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "gtceu:ingot_casting_mold"
           }
         }
         chance: 0
         tierChanceBoost: 0
       }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "tfc:brick/rhyolite"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
 }

```


</details>

<details>
<summary>gtceu/alloy_smelter/schist_brick</summary>

```diff
 {
   type: "gtceu:alloy_smelter"
-  duration: 120
+  duration: 60
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "tfc:rock/loose/schist"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "gtceu:ingot_casting_mold"
           }
         }
         chance: 0
         tierChanceBoost: 0
       }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "tfc:brick/schist"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
 }

```


</details>

<details>
<summary>gtceu/alloy_smelter/shale_brick</summary>

```diff
 {
   type: "gtceu:alloy_smelter"
-  duration: 120
+  duration: 60
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "tfc:rock/loose/shale"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "gtceu:ingot_casting_mold"
           }
         }
         chance: 0
         tierChanceBoost: 0
       }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "tfc:brick/shale"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
 }

```


</details>

<details>
<summary>gtceu/alloy_smelter/slate_brick</summary>

```diff
 {
   type: "gtceu:alloy_smelter"
-  duration: 120
+  duration: 60
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "tfc:rock/loose/slate"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "gtceu:ingot_casting_mold"
           }
         }
         chance: 0
         tierChanceBoost: 0
       }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "tfc:brick/slate"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_aluminium_buzzsaw</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 593
+  duration: 1126
   inputs: {
     fluid: [
       {
         content: {
-          amount: 593
+          amount: 1126
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:aluminium_buzzsaw"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tungsten_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:aluminium_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:tungsten_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_bisalloy_400_buzzsaw</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 685
+  duration: 1218
   inputs: {
     fluid: [
       {
         content: {
-          amount: 685
+          amount: 1218
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gcyr:bisalloy_400_buzzsaw"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tungsten_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gcyr:bisalloy_400_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:tungsten_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_blue_steel_buzzsaw</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 789
+  duration: 1322
   inputs: {
     fluid: [
       {
         content: {
-          amount: 789
+          amount: 1322
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:blue_steel_buzzsaw"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tungsten_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:blue_steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:tungsten_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_bronze_buzzsaw</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 793
+  duration: 1326
   inputs: {
     fluid: [
       {
         content: {
-          amount: 793
+          amount: 1326
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:bronze_buzzsaw"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tungsten_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:bronze_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:tungsten_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_cleanroom</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 2576
+  duration: 2372
   inputs: {
     fluid: [
       {
         content: {
-          amount: 2576
+          amount: 2372
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "gtceu:cleanroom"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 10
           ingredient: {
             item: "firmalife:metal/ingot/stainless_steel"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 8
           ingredient: {
             item: "gtceu:electrum_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 6
           ingredient: {
             item: "gtceu:zinc_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
-            item: "gtceu:silver_ingot"
+            item: "gtceu:steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_cobalt_brass_buzzsaw</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 721
+  duration: 1254
   inputs: {
     fluid: [
       {
         content: {
-          amount: 721
+          amount: 1254
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:cobalt_brass_buzzsaw"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tungsten_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:cobalt_brass_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:tungsten_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_damascus_steel_buzzsaw</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 713
+  duration: 1246
   inputs: {
     fluid: [
       {
         content: {
-          amount: 713
+          amount: 1246
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:damascus_steel_buzzsaw"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tungsten_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:damascus_steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:tungsten_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_diamond_buzzsaw</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 495
+  duration: 1086
   inputs: {
     fluid: [
       {
         content: {
-          amount: 495
+          amount: 1086
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:diamond_buzzsaw"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tungsten_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 2
           ingredient: {
-            item: "gtceu:small_carbon_dust"
+            item: "gtceu:tungsten_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:neodymium_nugget"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_duranium_buzzsaw</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 1689
+  duration: 2222
   inputs: {
     fluid: [
       {
         content: {
-          amount: 1689
+          amount: 2222
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:duranium_buzzsaw"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tungsten_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:duranium_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:tungsten_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_ev_aluminium_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 525
+  duration: 801
   inputs: {
     fluid: [
       {
         content: {
-          amount: 525
+          amount: 801
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:ev_aluminium_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:titanium_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 4
+          count: 6
           ingredient: {
             item: "gtceu:aluminium_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:kanthal_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_ev_bisalloy_400_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 617
+  duration: 841
   inputs: {
     fluid: [
       {
         content: {
-          amount: 617
+          amount: 841
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gcyr:ev_bisalloy_400_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:titanium_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gcyr:bisalloy_400_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:kanthal_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_ev_blue_steel_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 721
+  duration: 945
   inputs: {
     fluid: [
       {
         content: {
-          amount: 721
+          amount: 945
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:ev_blue_steel_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:titanium_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:blue_steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:kanthal_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_ev_bronze_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 725
+  duration: 949
   inputs: {
     fluid: [
       {
         content: {
-          amount: 725
+          amount: 949
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:ev_bronze_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:titanium_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:bronze_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:kanthal_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_ev_cobalt_brass_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 653
+  duration: 877
   inputs: {
     fluid: [
       {
         content: {
-          amount: 653
+          amount: 877
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:ev_cobalt_brass_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:titanium_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:cobalt_brass_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:kanthal_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_ev_damascus_steel_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 645
+  duration: 869
   inputs: {
     fluid: [
       {
         content: {
-          amount: 645
+          amount: 869
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:ev_damascus_steel_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:titanium_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:damascus_steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:kanthal_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_ev_diamond_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 427
+  duration: 697
   inputs: {
     fluid: [
       {
         content: {
-          amount: 427
+          amount: 697
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:ev_diamond_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:titanium_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 2
           ingredient: {
-            item: "gtceu:small_carbon_dust"
+            item: "gtceu:aluminium_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:kanthal_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_ev_duranium_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 1621
+  duration: 1845
   inputs: {
     fluid: [
       {
         content: {
-          amount: 1621
+          amount: 1845
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:ev_duranium_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:titanium_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:duranium_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:kanthal_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_ev_hsse_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 745
+  duration: 969
   inputs: {
     fluid: [
       {
         content: {
-          amount: 745
+          amount: 969
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:ev_hsse_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:titanium_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:hsse_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:kanthal_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_ev_invar_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 645
+  duration: 869
   inputs: {
     fluid: [
       {
         content: {
-          amount: 645
+          amount: 869
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:ev_invar_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:titanium_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:invar_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:kanthal_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_ev_iron_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 645
+  duration: 869
   inputs: {
     fluid: [
       {
         content: {
-          amount: 645
+          amount: 869
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:ev_iron_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:titanium_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:wrought_iron_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:kanthal_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_ev_naquadah_alloy_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 1985
+  duration: 2209
   inputs: {
     fluid: [
       {
         content: {
-          amount: 1985
+          amount: 2209
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:ev_naquadah_alloy_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:titanium_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:naquadah_alloy_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:kanthal_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_ev_neutronium_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 4421
+  duration: 4645
   inputs: {
     fluid: [
       {
         content: {
-          amount: 4421
+          amount: 4645
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:ev_neutronium_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:titanium_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:neutronium_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:kanthal_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_ev_red_steel_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 697
+  duration: 921
   inputs: {
     fluid: [
       {
         content: {
-          amount: 697
+          amount: 921
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:ev_red_steel_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:titanium_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:red_steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:kanthal_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_ev_rose_gold_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 1097
+  duration: 1321
   inputs: {
     fluid: [
       {
         content: {
-          amount: 1097
+          amount: 1321
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:ev_rose_gold_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:titanium_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:rose_gold_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:kanthal_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_ev_stainless_steel_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 641
+  duration: 865
   inputs: {
     fluid: [
       {
         content: {
-          amount: 641
+          amount: 865
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:ev_stainless_steel_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:titanium_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "firmalife:metal/ingot/stainless_steel"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:kanthal_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_ev_steel_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 645
+  duration: 921
   inputs: {
     fluid: [
       {
         content: {
-          amount: 645
+          amount: 921
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:ev_steel_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 8
           ingredient: {
             item: "gtceu:steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:titanium_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:kanthal_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:aluminium_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_ev_sterling_silver_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 813
+  duration: 1037
   inputs: {
     fluid: [
       {
         content: {
-          amount: 813
+          amount: 1037
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:ev_sterling_silver_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:titanium_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:sterling_silver_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:kanthal_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_ev_titanium_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 613
+  duration: 884
   inputs: {
     fluid: [
       {
         content: {
-          amount: 613
+          amount: 884
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:ev_titanium_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
-      {
-        content: {
-          type: "gtceu:sized"
-          count: 8
-          ingredient: {
-            item: "gtceu:titanium_ingot"
-          }
-        }
-        chance: 1
-        tierChanceBoost: 0
-      }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
-            item: "gtceu:titanium_nugget"
+            item: "gtceu:titanium_block"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:kanthal_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:aluminium_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_ev_tungsten_carbide_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 809
+  duration: 1033
   inputs: {
     fluid: [
       {
         content: {
-          amount: 809
+          amount: 1033
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:ev_tungsten_carbide_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:titanium_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:tungsten_carbide_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:kanthal_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_ev_tungsten_steel_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 897
+  duration: 1121
   inputs: {
     fluid: [
       {
         content: {
-          amount: 897
+          amount: 1121
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:ev_tungsten_steel_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:titanium_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:tungsten_steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:kanthal_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_ev_ultimet_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 665
+  duration: 889
   inputs: {
     fluid: [
       {
         content: {
-          amount: 665
+          amount: 889
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:ev_ultimet_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:titanium_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:ultimet_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:kanthal_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_ev_vanadium_steel_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 641
+  duration: 865
   inputs: {
     fluid: [
       {
         content: {
-          amount: 641
+          amount: 865
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:ev_vanadium_steel_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:titanium_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:vanadium_steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:kanthal_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_ev_wrought_iron_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 645
+  duration: 869
   inputs: {
     fluid: [
       {
         content: {
-          amount: 645
+          amount: 869
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:ev_wrought_iron_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:titanium_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:wrought_iron_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:kanthal_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_filter_casing</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 1197
+  duration: 1160
   inputs: {
     fluid: [
       {
         content: {
-          amount: 1197
+          amount: 1160
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "gtceu:filter_casing"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "gtceu:steel_block"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 6
           ingredient: {
             item: "gtceu:zinc_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:cupronickel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
-            item: "gtceu:annealed_copper_ingot"
+            item: "gtceu:aluminium_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_hsse_buzzsaw</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 813
+  duration: 1346
   inputs: {
     fluid: [
       {
         content: {
-          amount: 813
+          amount: 1346
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:hsse_buzzsaw"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tungsten_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:hsse_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:tungsten_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_hv_aluminium_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 554
+  duration: 1238
   inputs: {
     fluid: [
       {
         content: {
-          amount: 554
+          amount: 1238
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:hv_aluminium_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:stainless_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 4
+          count: 40
           ingredient: {
-            item: "gtceu:steel_ingot"
+            item: "gtceu:steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:aluminium_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:electrum_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_hv_aluminium_wrench</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 355
+  duration: 1203
   inputs: {
     fluid: [
       {
         content: {
-          amount: 355
+          amount: 1203
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:hv_aluminium_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:stainless_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:aluminium_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 4
+          count: 2
           ingredient: {
-            item: "gtceu:steel_nugget"
+            item: "gtceu:silver_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:electrum_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_hv_bisalloy_400_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 646
+  duration: 1330
   inputs: {
     fluid: [
       {
         content: {
-          amount: 646
+          amount: 1330
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gcyr:hv_bisalloy_400_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:stainless_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 4
+          count: 40
           ingredient: {
-            item: "gtceu:steel_ingot"
+            item: "gtceu:steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gcyr:bisalloy_400_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:electrum_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_hv_bisalloy_400_wrench</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 447
+  duration: 1295
   inputs: {
     fluid: [
       {
         content: {
-          amount: 447
+          amount: 1295
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gcyr:hv_bisalloy_400_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:stainless_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gcyr:bisalloy_400_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 4
+          count: 2
           ingredient: {
-            item: "gtceu:steel_nugget"
+            item: "gtceu:silver_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:electrum_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_hv_blue_steel_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 750
+  duration: 1434
   inputs: {
     fluid: [
       {
         content: {
-          amount: 750
+          amount: 1434
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:hv_blue_steel_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:stainless_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:blue_steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
-            item: "gtceu:steel_ingot"
+            item: "gtceu:electrum_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 40
+          ingredient: {
+            item: "gtceu:steel_nugget"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_hv_blue_steel_wrench</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 551
+  duration: 1399
   inputs: {
     fluid: [
       {
         content: {
-          amount: 551
+          amount: 1399
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:hv_blue_steel_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:stainless_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:blue_steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 4
+          count: 2
           ingredient: {
-            item: "gtceu:steel_nugget"
+            item: "gtceu:silver_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:electrum_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_hv_bronze_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 754
+  duration: 1438
   inputs: {
     fluid: [
       {
         content: {
-          amount: 754
+          amount: 1438
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:hv_bronze_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:stainless_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:bronze_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
-            item: "gtceu:steel_ingot"
+            item: "gtceu:electrum_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 40
+          ingredient: {
+            item: "gtceu:steel_nugget"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_hv_bronze_wrench</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 555
+  duration: 1403
   inputs: {
     fluid: [
       {
         content: {
-          amount: 555
+          amount: 1403
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:hv_bronze_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:stainless_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:bronze_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 4
+          count: 2
           ingredient: {
-            item: "gtceu:steel_nugget"
+            item: "gtceu:silver_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:electrum_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_hv_cobalt_brass_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 682
+  duration: 1366
   inputs: {
     fluid: [
       {
         content: {
-          amount: 682
+          amount: 1366
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:hv_cobalt_brass_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:stainless_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:cobalt_brass_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
-            item: "gtceu:steel_ingot"
+            item: "gtceu:electrum_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 40
+          ingredient: {
+            item: "gtceu:steel_nugget"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_hv_cobalt_brass_wrench</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 483
+  duration: 1331
   inputs: {
     fluid: [
       {
         content: {
-          amount: 483
+          amount: 1331
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:hv_cobalt_brass_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:stainless_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:cobalt_brass_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 4
+          count: 2
           ingredient: {
-            item: "gtceu:steel_nugget"
+            item: "gtceu:silver_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:electrum_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_hv_damascus_steel_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 674
+  duration: 1358
   inputs: {
     fluid: [
       {
         content: {
-          amount: 674
+          amount: 1358
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:hv_damascus_steel_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:stainless_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:damascus_steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
-            item: "gtceu:steel_ingot"
+            item: "gtceu:electrum_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 40
+          ingredient: {
+            item: "gtceu:steel_nugget"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_hv_damascus_steel_wrench</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 475
+  duration: 1323
   inputs: {
     fluid: [
       {
         content: {
-          amount: 475
+          amount: 1323
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:hv_damascus_steel_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:stainless_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:damascus_steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
-            item: "gtceu:steel_nugget"
+            item: "gtceu:electrum_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:silver_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_hv_diamond_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 456
+  duration: 1348
   inputs: {
     fluid: [
       {
         content: {
-          amount: 456
+          amount: 1348
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:hv_diamond_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:stainless_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
-            item: "gtceu:steel_ingot"
+            item: "gtceu:electrum_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 2
           ingredient: {
-            item: "gtceu:small_carbon_dust"
+            item: "gtceu:silver_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 40
+          ingredient: {
+            item: "gtceu:steel_nugget"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_hv_diamond_wrench</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 257
+  duration: 1148
   inputs: {
     fluid: [
       {
         content: {
-          amount: 257
+          amount: 1148
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:hv_diamond_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:stainless_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
-            item: "gtceu:steel_nugget"
+            item: "gtceu:electrum_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 2
           ingredient: {
-            item: "gtceu:small_carbon_dust"
+            item: "gtceu:silver_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 8
+          ingredient: {
+            item: "gtceu:steel_nugget"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_hv_duranium_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 1650
+  duration: 2334
   inputs: {
     fluid: [
       {
         content: {
-          amount: 1650
+          amount: 2334
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:hv_duranium_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:stainless_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 4
+          count: 40
           ingredient: {
-            item: "gtceu:steel_ingot"
+            item: "gtceu:steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:duranium_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:electrum_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_hv_duranium_wrench</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 1451
+  duration: 2299
   inputs: {
     fluid: [
       {
         content: {
-          amount: 1451
+          amount: 2299
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:hv_duranium_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:stainless_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:duranium_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 4
+          count: 2
           ingredient: {
-            item: "gtceu:steel_nugget"
+            item: "gtceu:silver_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:electrum_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_hv_fluid_heater</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 2580
+  duration: 2328
   inputs: {
     fluid: [
       {
         content: {
-          amount: 2580
+          amount: 2328
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "gtceu:hv_fluid_heater"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "gtceu:steel_block"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 8
           ingredient: {
             item: "gtceu:electrum_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 8
           ingredient: {
             item: "firmalife:metal/ingot/stainless_steel"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
-            item: "gtceu:silver_ingot"
+            item: "gtceu:kanthal_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_hv_hsse_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 774
+  duration: 1458
   inputs: {
     fluid: [
       {
         content: {
-          amount: 774
+          amount: 1458
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:hv_hsse_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:stainless_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 4
+          count: 40
           ingredient: {
-            item: "gtceu:steel_ingot"
+            item: "gtceu:steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:hsse_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:electrum_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_hv_hsse_wrench</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 575
+  duration: 1423
   inputs: {
     fluid: [
       {
         content: {
-          amount: 575
+          amount: 1423
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:hv_hsse_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:stainless_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:hsse_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 4
+          count: 2
           ingredient: {
-            item: "gtceu:steel_nugget"
+            item: "gtceu:silver_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:electrum_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_hv_invar_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 674
+  duration: 1358
   inputs: {
     fluid: [
       {
         content: {
-          amount: 674
+          amount: 1358
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:hv_invar_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:stainless_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:invar_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
-            item: "gtceu:steel_ingot"
+            item: "gtceu:electrum_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 40
+          ingredient: {
+            item: "gtceu:steel_nugget"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_hv_invar_wrench</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 475
+  duration: 1323
   inputs: {
     fluid: [
       {
         content: {
-          amount: 475
+          amount: 1323
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:hv_invar_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:stainless_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:invar_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 4
+          count: 2
           ingredient: {
-            item: "gtceu:steel_nugget"
+            item: "gtceu:silver_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:electrum_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_hv_iron_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 674
+  duration: 1358
   inputs: {
     fluid: [
       {
         content: {
-          amount: 674
+          amount: 1358
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:hv_iron_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:stainless_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:wrought_iron_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
-            item: "gtceu:steel_ingot"
+            item: "gtceu:electrum_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 40
+          ingredient: {
+            item: "gtceu:steel_nugget"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_hv_iron_wrench</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 475
+  duration: 1323
   inputs: {
     fluid: [
       {
         content: {
-          amount: 475
+          amount: 1323
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:hv_iron_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:stainless_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:wrought_iron_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 4
+          count: 2
           ingredient: {
-            item: "gtceu:steel_nugget"
+            item: "gtceu:silver_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:electrum_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_hv_naquadah_alloy_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 2014
+  duration: 2698
   inputs: {
     fluid: [
       {
         content: {
-          amount: 2014
+          amount: 2698
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:hv_naquadah_alloy_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:stainless_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 4
+          count: 40
           ingredient: {
-            item: "gtceu:steel_ingot"
+            item: "gtceu:steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:naquadah_alloy_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:electrum_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_hv_naquadah_alloy_wrench</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 1815
+  duration: 2663
   inputs: {
     fluid: [
       {
         content: {
-          amount: 1815
+          amount: 2663
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:hv_naquadah_alloy_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:stainless_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:naquadah_alloy_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 4
+          count: 2
           ingredient: {
-            item: "gtceu:steel_nugget"
+            item: "gtceu:silver_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:electrum_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_hv_neutronium_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 4450
+  duration: 5134
   inputs: {
     fluid: [
       {
         content: {
-          amount: 4450
+          amount: 5134
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:hv_neutronium_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:stainless_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 4
+          count: 40
           ingredient: {
-            item: "gtceu:steel_ingot"
+            item: "gtceu:steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:neutronium_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:electrum_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_hv_neutronium_wrench</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 4251
+  duration: 5099
   inputs: {
     fluid: [
       {
         content: {
-          amount: 4251
+          amount: 5099
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:hv_neutronium_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:stainless_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:neutronium_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
-            item: "gtceu:steel_nugget"
+            item: "gtceu:electrum_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:silver_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_hv_red_steel_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 726
+  duration: 1410
   inputs: {
     fluid: [
       {
         content: {
-          amount: 726
+          amount: 1410
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:hv_red_steel_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:stainless_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 4
+          count: 40
           ingredient: {
-            item: "gtceu:steel_ingot"
+            item: "gtceu:steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:red_steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:electrum_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_hv_red_steel_wrench</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 527
+  duration: 1375
   inputs: {
     fluid: [
       {
         content: {
-          amount: 527
+          amount: 1375
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:hv_red_steel_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:stainless_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:red_steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 4
+          count: 2
           ingredient: {
-            item: "gtceu:steel_nugget"
+            item: "gtceu:silver_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:electrum_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_hv_rose_gold_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 1126
+  duration: 1810
   inputs: {
     fluid: [
       {
         content: {
-          amount: 1126
+          amount: 1810
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:hv_rose_gold_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:stainless_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:rose_gold_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
-            item: "gtceu:steel_ingot"
+            item: "gtceu:electrum_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 40
+          ingredient: {
+            item: "gtceu:steel_nugget"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_hv_rose_gold_wrench</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 927
+  duration: 1775
   inputs: {
     fluid: [
       {
         content: {
-          amount: 927
+          amount: 1775
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:hv_rose_gold_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:stainless_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:rose_gold_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 4
+          count: 2
           ingredient: {
-            item: "gtceu:steel_nugget"
+            item: "gtceu:silver_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:electrum_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_hv_stainless_steel_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 670
+  duration: 1561
   inputs: {
     fluid: [
       {
         content: {
-          amount: 670
+          amount: 1561
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:hv_stainless_steel_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
-      {
-        content: {
-          type: "gtceu:sized"
-          count: 8
-          ingredient: {
-            item: "firmalife:metal/ingot/stainless_steel"
-          }
-        }
-        chance: 1
-        tierChanceBoost: 0
-      }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
-            item: "gtceu:steel_ingot"
+            item: "gtceu:electrum_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
-            item: "gtceu:stainless_steel_nugget"
+            item: "gtceu:stainless_steel_block"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 40
+          ingredient: {
+            item: "gtceu:steel_nugget"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:silver_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_hv_stainless_steel_wrench</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 471
+  duration: 1362
   inputs: {
     fluid: [
       {
         content: {
-          amount: 471
+          amount: 1362
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:hv_stainless_steel_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
-      {
-        content: {
-          type: "gtceu:sized"
-          count: 8
-          ingredient: {
-            item: "firmalife:metal/ingot/stainless_steel"
-          }
-        }
-        chance: 1
-        tierChanceBoost: 0
-      }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
-            item: "gtceu:steel_nugget"
+            item: "gtceu:electrum_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
-            item: "gtceu:stainless_steel_nugget"
+            item: "gtceu:stainless_steel_block"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:silver_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 8
+          ingredient: {
+            item: "gtceu:steel_nugget"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_hv_steel_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 674
+  duration: 1547
   inputs: {
     fluid: [
       {
         content: {
-          amount: 674
+          amount: 1547
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:hv_steel_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 8
           ingredient: {
             item: "gtceu:steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:stainless_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:electrum_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:silver_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_hv_steel_wrench</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 475
+  duration: 1372
   inputs: {
     fluid: [
       {
         content: {
-          amount: 475
+          amount: 1372
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:hv_steel_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 40
+          count: 44
           ingredient: {
             item: "gtceu:steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:stainless_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:electrum_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:silver_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_hv_sterling_silver_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 842
+  duration: 1526
   inputs: {
     fluid: [
       {
         content: {
-          amount: 842
+          amount: 1526
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:hv_sterling_silver_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:stainless_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 4
+          count: 40
           ingredient: {
-            item: "gtceu:steel_ingot"
+            item: "gtceu:steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:sterling_silver_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:electrum_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_hv_sterling_silver_wrench</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 643
+  duration: 1491
   inputs: {
     fluid: [
       {
         content: {
-          amount: 643
+          amount: 1491
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:hv_sterling_silver_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:stainless_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:sterling_silver_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 4
+          count: 2
           ingredient: {
-            item: "gtceu:steel_nugget"
+            item: "gtceu:silver_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:electrum_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_hv_titanium_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 642
+  duration: 1326
   inputs: {
     fluid: [
       {
         content: {
-          amount: 642
+          amount: 1326
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:hv_titanium_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:stainless_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:titanium_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
-            item: "gtceu:steel_ingot"
+            item: "gtceu:electrum_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 40
+          ingredient: {
+            item: "gtceu:steel_nugget"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_hv_titanium_wrench</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 443
+  duration: 1291
   inputs: {
     fluid: [
       {
         content: {
-          amount: 443
+          amount: 1291
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:hv_titanium_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:stainless_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:titanium_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 4
+          count: 2
           ingredient: {
-            item: "gtceu:steel_nugget"
+            item: "gtceu:silver_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:electrum_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_hv_tungsten_carbide_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 838
+  duration: 1522
   inputs: {
     fluid: [
       {
         content: {
-          amount: 838
+          amount: 1522
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:hv_tungsten_carbide_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:stainless_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 4
+          count: 40
           ingredient: {
-            item: "gtceu:steel_ingot"
+            item: "gtceu:steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:tungsten_carbide_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:electrum_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_hv_tungsten_carbide_wrench</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 639
+  duration: 1487
   inputs: {
     fluid: [
       {
         content: {
-          amount: 639
+          amount: 1487
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:hv_tungsten_carbide_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:stainless_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:tungsten_carbide_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 4
+          count: 2
           ingredient: {
-            item: "gtceu:steel_nugget"
+            item: "gtceu:silver_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:electrum_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_hv_tungsten_steel_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 926
+  duration: 1610
   inputs: {
     fluid: [
       {
         content: {
-          amount: 926
+          amount: 1610
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:hv_tungsten_steel_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:stainless_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 4
+          count: 40
           ingredient: {
-            item: "gtceu:steel_ingot"
+            item: "gtceu:steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:tungsten_steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:electrum_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_hv_tungsten_steel_wrench</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 727
+  duration: 1575
   inputs: {
     fluid: [
       {
         content: {
-          amount: 727
+          amount: 1575
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:hv_tungsten_steel_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:stainless_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:tungsten_steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 4
+          count: 2
           ingredient: {
-            item: "gtceu:steel_nugget"
+            item: "gtceu:silver_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:electrum_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_hv_ultimet_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 694
+  duration: 1378
   inputs: {
     fluid: [
       {
         content: {
-          amount: 694
+          amount: 1378
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:hv_ultimet_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:stainless_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:ultimet_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
-            item: "gtceu:steel_ingot"
+            item: "gtceu:electrum_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 40
+          ingredient: {
+            item: "gtceu:steel_nugget"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_hv_ultimet_wrench</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 495
+  duration: 1343
   inputs: {
     fluid: [
       {
         content: {
-          amount: 495
+          amount: 1343
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:hv_ultimet_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:stainless_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:ultimet_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 4
+          count: 2
           ingredient: {
-            item: "gtceu:steel_nugget"
+            item: "gtceu:silver_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:electrum_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_hv_vanadium_steel_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 670
+  duration: 1354
   inputs: {
     fluid: [
       {
         content: {
-          amount: 670
+          amount: 1354
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:hv_vanadium_steel_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:stainless_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 4
+          count: 40
           ingredient: {
-            item: "gtceu:steel_ingot"
+            item: "gtceu:steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:vanadium_steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:electrum_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_hv_vanadium_steel_wrench</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 471
+  duration: 1319
   inputs: {
     fluid: [
       {
         content: {
-          amount: 471
+          amount: 1319
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:hv_vanadium_steel_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:stainless_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:vanadium_steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 4
+          count: 2
           ingredient: {
-            item: "gtceu:steel_nugget"
+            item: "gtceu:silver_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:electrum_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_hv_wrought_iron_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 674
+  duration: 1358
   inputs: {
     fluid: [
       {
         content: {
-          amount: 674
+          amount: 1358
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:hv_wrought_iron_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:stainless_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:wrought_iron_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
-            item: "gtceu:steel_ingot"
+            item: "gtceu:electrum_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 40
+          ingredient: {
+            item: "gtceu:steel_nugget"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_hv_wrought_iron_wrench</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 475
+  duration: 1323
   inputs: {
     fluid: [
       {
         content: {
-          amount: 475
+          amount: 1323
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:hv_wrought_iron_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:stainless_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:wrought_iron_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 4
+          count: 2
           ingredient: {
-            item: "gtceu:steel_nugget"
+            item: "gtceu:silver_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:electrum_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_invar_buzzsaw</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 713
+  duration: 1246
   inputs: {
     fluid: [
       {
         content: {
-          amount: 713
+          amount: 1246
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:invar_buzzsaw"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tungsten_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:invar_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:tungsten_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_iron_buzzsaw</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 713
+  duration: 1246
   inputs: {
     fluid: [
       {
         content: {
-          amount: 713
+          amount: 1246
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:iron_buzzsaw"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tungsten_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:wrought_iron_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:tungsten_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_iv_aluminium_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 817
+  duration: 984
   inputs: {
     fluid: [
       {
         content: {
-          amount: 817
+          amount: 984
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:iv_aluminium_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tungsten_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:aluminium_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_iv_aluminium_wrench</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 618
+  duration: 1126
   inputs: {
     fluid: [
       {
         content: {
-          amount: 618
+          amount: 1126
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:iv_aluminium_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tungsten_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:aluminium_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
-            item: "gtceu:steel_nugget"
+            item: "gtceu:graphene_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:tungsten_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_iv_bisalloy_400_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 909
+  duration: 1076
   inputs: {
     fluid: [
       {
         content: {
-          amount: 909
+          amount: 1076
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gcyr:iv_bisalloy_400_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tungsten_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gcyr:bisalloy_400_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_iv_bisalloy_400_wrench</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 710
+  duration: 1218
   inputs: {
     fluid: [
       {
         content: {
-          amount: 710
+          amount: 1218
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gcyr:iv_bisalloy_400_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tungsten_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gcyr:bisalloy_400_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
-            item: "gtceu:steel_nugget"
+            item: "gtceu:graphene_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:tungsten_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_iv_blue_steel_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 1013
+  duration: 1180
   inputs: {
     fluid: [
       {
         content: {
-          amount: 1013
+          amount: 1180
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:iv_blue_steel_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tungsten_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:blue_steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_iv_blue_steel_wrench</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 814
+  duration: 1322
   inputs: {
     fluid: [
       {
         content: {
-          amount: 814
+          amount: 1322
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:iv_blue_steel_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tungsten_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:blue_steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
-            item: "gtceu:steel_nugget"
+            item: "gtceu:graphene_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:tungsten_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_iv_bronze_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 1017
+  duration: 1184
   inputs: {
     fluid: [
       {
         content: {
-          amount: 1017
+          amount: 1184
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:iv_bronze_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tungsten_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:bronze_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_iv_bronze_wrench</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 818
+  duration: 1326
   inputs: {
     fluid: [
       {
         content: {
-          amount: 818
+          amount: 1326
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:iv_bronze_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tungsten_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:bronze_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
-            item: "gtceu:steel_nugget"
+            item: "gtceu:graphene_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:tungsten_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_iv_cobalt_brass_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 945
+  duration: 1112
   inputs: {
     fluid: [
       {
         content: {
-          amount: 945
+          amount: 1112
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:iv_cobalt_brass_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tungsten_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:cobalt_brass_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_iv_cobalt_brass_wrench</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 746
+  duration: 1254
   inputs: {
     fluid: [
       {
         content: {
-          amount: 746
+          amount: 1254
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:iv_cobalt_brass_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tungsten_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:cobalt_brass_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
-            item: "gtceu:steel_nugget"
+            item: "gtceu:graphene_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:tungsten_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_iv_damascus_steel_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 937
+  duration: 1104
   inputs: {
     fluid: [
       {
         content: {
-          amount: 937
+          amount: 1104
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:iv_damascus_steel_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tungsten_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:damascus_steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_iv_damascus_steel_wrench</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 738
+  duration: 1246
   inputs: {
     fluid: [
       {
         content: {
-          amount: 738
+          amount: 1246
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:iv_damascus_steel_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tungsten_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:damascus_steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
-            item: "gtceu:steel_nugget"
+            item: "gtceu:graphene_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:tungsten_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_iv_diamond_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 719
+  duration: 1246
   inputs: {
     fluid: [
       {
         content: {
-          amount: 719
+          amount: 1246
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:iv_diamond_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tungsten_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 2
           ingredient: {
-            item: "gtceu:small_carbon_dust"
+            item: "gtceu:tungsten_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_iv_diamond_wrench</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 520
+  duration: 1086
   inputs: {
     fluid: [
       {
         content: {
-          amount: 520
+          amount: 1086
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:iv_diamond_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tungsten_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
-            item: "gtceu:steel_nugget"
+            item: "gtceu:graphene_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 2
           ingredient: {
-            item: "gtceu:small_carbon_dust"
+            item: "gtceu:tungsten_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:neodymium_nugget"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_iv_duranium_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 1913
+  duration: 2080
   inputs: {
     fluid: [
       {
         content: {
-          amount: 1913
+          amount: 2080
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:iv_duranium_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tungsten_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:duranium_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_iv_duranium_wrench</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 1714
+  duration: 2222
   inputs: {
     fluid: [
       {
         content: {
-          amount: 1714
+          amount: 2222
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:iv_duranium_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tungsten_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:duranium_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
-            item: "gtceu:steel_nugget"
+            item: "gtceu:graphene_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:tungsten_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_iv_hsse_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 1037
+  duration: 1204
   inputs: {
     fluid: [
       {
         content: {
-          amount: 1037
+          amount: 1204
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:iv_hsse_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tungsten_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:hsse_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_iv_hsse_wrench</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 838
+  duration: 1346
   inputs: {
     fluid: [
       {
         content: {
-          amount: 838
+          amount: 1346
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:iv_hsse_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tungsten_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:hsse_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
-            item: "gtceu:steel_nugget"
+            item: "gtceu:graphene_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:tungsten_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_iv_invar_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 937
+  duration: 1104
   inputs: {
     fluid: [
       {
         content: {
-          amount: 937
+          amount: 1104
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:iv_invar_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tungsten_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:invar_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_iv_invar_wrench</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 738
+  duration: 1246
   inputs: {
     fluid: [
       {
         content: {
-          amount: 738
+          amount: 1246
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:iv_invar_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tungsten_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:invar_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
-            item: "gtceu:steel_nugget"
+            item: "gtceu:graphene_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:tungsten_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_iv_iron_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 937
+  duration: 1104
   inputs: {
     fluid: [
       {
         content: {
-          amount: 937
+          amount: 1104
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:iv_iron_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tungsten_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:wrought_iron_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_iv_iron_wrench</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 738
+  duration: 1246
   inputs: {
     fluid: [
       {
         content: {
-          amount: 738
+          amount: 1246
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:iv_iron_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tungsten_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:wrought_iron_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
-            item: "gtceu:steel_nugget"
+            item: "gtceu:graphene_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:tungsten_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_iv_naquadah_alloy_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 2277
+  duration: 2444
   inputs: {
     fluid: [
       {
         content: {
-          amount: 2277
+          amount: 2444
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:iv_naquadah_alloy_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tungsten_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:naquadah_alloy_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_iv_naquadah_alloy_wrench</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 2078
+  duration: 2586
   inputs: {
     fluid: [
       {
         content: {
-          amount: 2078
+          amount: 2586
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:iv_naquadah_alloy_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tungsten_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:naquadah_alloy_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
-            item: "gtceu:steel_nugget"
+            item: "gtceu:graphene_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:tungsten_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_iv_neutronium_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 4713
+  duration: 4880
   inputs: {
     fluid: [
       {
         content: {
-          amount: 4713
+          amount: 4880
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:iv_neutronium_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tungsten_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:neutronium_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_iv_neutronium_wrench</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 4514
+  duration: 5022
   inputs: {
     fluid: [
       {
         content: {
-          amount: 4514
+          amount: 5022
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:iv_neutronium_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tungsten_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:neutronium_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
-            item: "gtceu:steel_nugget"
+            item: "gtceu:graphene_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:tungsten_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_iv_red_steel_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 989
+  duration: 1156
   inputs: {
     fluid: [
       {
         content: {
-          amount: 989
+          amount: 1156
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:iv_red_steel_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tungsten_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:red_steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_iv_red_steel_wrench</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 790
+  duration: 1298
   inputs: {
     fluid: [
       {
         content: {
-          amount: 790
+          amount: 1298
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:iv_red_steel_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tungsten_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:red_steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 4
+          count: 2
           ingredient: {
-            item: "gtceu:steel_nugget"
+            item: "gtceu:tungsten_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_iv_rose_gold_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 1389
+  duration: 1556
   inputs: {
     fluid: [
       {
         content: {
-          amount: 1389
+          amount: 1556
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:iv_rose_gold_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tungsten_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:rose_gold_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_iv_rose_gold_wrench</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 1190
+  duration: 1698
   inputs: {
     fluid: [
       {
         content: {
-          amount: 1190
+          amount: 1698
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:iv_rose_gold_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tungsten_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:rose_gold_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
-            item: "gtceu:steel_nugget"
+            item: "gtceu:graphene_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:tungsten_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_iv_stainless_steel_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 933
+  duration: 1100
   inputs: {
     fluid: [
       {
         content: {
-          amount: 933
+          amount: 1100
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:iv_stainless_steel_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tungsten_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "firmalife:metal/ingot/stainless_steel"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_iv_stainless_steel_wrench</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 734
+  duration: 1242
   inputs: {
     fluid: [
       {
         content: {
-          amount: 734
+          amount: 1242
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:iv_stainless_steel_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tungsten_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "firmalife:metal/ingot/stainless_steel"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
-            item: "gtceu:steel_nugget"
+            item: "gtceu:graphene_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:tungsten_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_iv_steel_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 937
+  duration: 1470
   inputs: {
     fluid: [
       {
         content: {
-          amount: 937
+          amount: 1470
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:iv_steel_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 8
           ingredient: {
             item: "gtceu:steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tungsten_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:tungsten_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_iv_steel_wrench</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 738
+  duration: 1271
   inputs: {
     fluid: [
       {
         content: {
-          amount: 738
+          amount: 1271
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:iv_steel_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 40
           ingredient: {
             item: "gtceu:steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tungsten_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:tungsten_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_iv_sterling_silver_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 1105
+  duration: 1272
   inputs: {
     fluid: [
       {
         content: {
-          amount: 1105
+          amount: 1272
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:iv_sterling_silver_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tungsten_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:sterling_silver_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_iv_sterling_silver_wrench</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 906
+  duration: 1414
   inputs: {
     fluid: [
       {
         content: {
-          amount: 906
+          amount: 1414
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:iv_sterling_silver_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tungsten_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:sterling_silver_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
-            item: "gtceu:steel_nugget"
+            item: "gtceu:graphene_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:tungsten_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_iv_titanium_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 905
+  duration: 1072
   inputs: {
     fluid: [
       {
         content: {
-          amount: 905
+          amount: 1072
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:iv_titanium_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tungsten_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:titanium_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_iv_titanium_wrench</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 706
+  duration: 1214
   inputs: {
     fluid: [
       {
         content: {
-          amount: 706
+          amount: 1214
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:iv_titanium_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tungsten_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:titanium_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
-            item: "gtceu:steel_nugget"
+            item: "gtceu:graphene_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:tungsten_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_iv_tungsten_carbide_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 1101
+  duration: 1268
   inputs: {
     fluid: [
       {
         content: {
-          amount: 1101
+          amount: 1268
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:iv_tungsten_carbide_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tungsten_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:tungsten_carbide_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_iv_tungsten_carbide_wrench</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 902
+  duration: 1410
   inputs: {
     fluid: [
       {
         content: {
-          amount: 902
+          amount: 1410
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:iv_tungsten_carbide_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tungsten_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:tungsten_carbide_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 4
+          count: 2
           ingredient: {
-            item: "gtceu:steel_nugget"
+            item: "gtceu:tungsten_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_iv_tungsten_steel_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 1189
+  duration: 1709
   inputs: {
     fluid: [
       {
         content: {
-          amount: 1189
+          amount: 1709
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:iv_tungsten_steel_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
-      {
-        content: {
-          type: "gtceu:sized"
-          count: 8
-          ingredient: {
-            item: "gtceu:tungsten_steel_ingot"
-          }
-        }
-        chance: 1
-        tierChanceBoost: 0
-      }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
-            item: "gtceu:tungsten_steel_nugget"
+            item: "gtceu:tungsten_steel_block"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:tungsten_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_iv_tungsten_steel_wrench</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 990
+  duration: 1549
   inputs: {
     fluid: [
       {
         content: {
-          amount: 990
+          amount: 1549
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:iv_tungsten_steel_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
-      {
-        content: {
-          type: "gtceu:sized"
-          count: 8
-          ingredient: {
-            item: "gtceu:tungsten_steel_ingot"
-          }
-        }
-        chance: 1
-        tierChanceBoost: 0
-      }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
-            item: "gtceu:steel_nugget"
+            item: "gtceu:graphene_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
-            item: "gtceu:tungsten_steel_nugget"
+            item: "gtceu:tungsten_steel_block"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:tungsten_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:neodymium_nugget"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_iv_ultimet_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 957
+  duration: 1124
   inputs: {
     fluid: [
       {
         content: {
-          amount: 957
+          amount: 1124
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:iv_ultimet_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tungsten_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:ultimet_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_iv_ultimet_wrench</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 758
+  duration: 1266
   inputs: {
     fluid: [
       {
         content: {
-          amount: 758
+          amount: 1266
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:iv_ultimet_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tungsten_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:ultimet_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 4
+          count: 2
           ingredient: {
-            item: "gtceu:steel_nugget"
+            item: "gtceu:tungsten_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_iv_vanadium_steel_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 933
+  duration: 1100
   inputs: {
     fluid: [
       {
         content: {
-          amount: 933
+          amount: 1100
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:iv_vanadium_steel_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tungsten_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:vanadium_steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_iv_vanadium_steel_wrench</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 734
+  duration: 1242
   inputs: {
     fluid: [
       {
         content: {
-          amount: 734
+          amount: 1242
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:iv_vanadium_steel_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tungsten_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:vanadium_steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
-            item: "gtceu:steel_nugget"
+            item: "gtceu:graphene_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:tungsten_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_iv_wrought_iron_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 937
+  duration: 1104
   inputs: {
     fluid: [
       {
         content: {
-          amount: 937
+          amount: 1104
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:iv_wrought_iron_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tungsten_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:wrought_iron_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_iv_wrought_iron_wrench</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 738
+  duration: 1246
   inputs: {
     fluid: [
       {
         content: {
-          amount: 738
+          amount: 1246
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:iv_wrought_iron_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tungsten_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:wrought_iron_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
-            item: "gtceu:steel_nugget"
+            item: "gtceu:graphene_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:tungsten_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_large_electromagnet</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 1495
+  duration: 1647
   inputs: {
     fluid: [
       {
         content: {
-          amount: 1495
+          amount: 1647
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "gtceu:large_electromagnet"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 12
           ingredient: {
             item: "gtceu:graphene_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 40
           ingredient: {
             item: "gtceu:tungsten_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:blue_steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 2
           ingredient: {
-            item: "gtceu:tungsten_steel_ingot"
+            item: "gtceu:platinum_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_large_sifting_funnel</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 5488
+  duration: 5504
   inputs: {
     fluid: [
       {
         content: {
-          amount: 5488
+          amount: 5504
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "gtceu:large_sifting_funnel"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 24
           ingredient: {
             item: "gtceu:tungsten_steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 16
           ingredient: {
             item: "gtceu:graphene_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 12
           ingredient: {
             item: "gtceu:tungsten_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
-            item: "gtceu:hsla_steel_ingot"
+            item: "gtceu:zinc_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_lv_aluminium_chainsaw</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 531
+  duration: 706
   inputs: {
     fluid: [
       {
         content: {
-          amount: 531
+          amount: 706
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_aluminium_chainsaw"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 8
           ingredient: {
             item: "gtceu:steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 2
           ingredient: {
             item: "gtceu:aluminium_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 5
+          count: 13
           ingredient: {
-            item: "gtceu:steel_nugget"
+            item: "gtceu:wrought_iron_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:annealed_copper_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_lv_aluminium_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 558
+  duration: 758
   inputs: {
     fluid: [
       {
         content: {
-          amount: 558
+          amount: 758
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_aluminium_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 8
           ingredient: {
             item: "gtceu:steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:aluminium_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 1
+          count: 2
           ingredient: {
-            item: "gtceu:steel_nugget"
+            item: "gtceu:annealed_copper_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 13
+          ingredient: {
+            item: "gtceu:wrought_iron_nugget"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_lv_aluminium_screwdriver</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 515
+  duration: 1048
   inputs: {
     fluid: [
       {
         content: {
-          amount: 515
+          amount: 1048
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_aluminium_screwdriver"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tungsten_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "gtceu:aluminium_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:tungsten_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_lv_aluminium_wrench</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 359
+  duration: 566
   inputs: {
     fluid: [
       {
         content: {
-          amount: 359
+          amount: 566
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_aluminium_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 41
           ingredient: {
             item: "gtceu:steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:aluminium_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:annealed_copper_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 13
+          ingredient: {
+            item: "gtceu:wrought_iron_nugget"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_lv_bisalloy_400_chainsaw</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 577
+  duration: 752
   inputs: {
     fluid: [
       {
         content: {
-          amount: 577
+          amount: 752
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gcyr:lv_bisalloy_400_chainsaw"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 8
           ingredient: {
             item: "gtceu:steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 2
           ingredient: {
             item: "gcyr:bisalloy_400_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 5
+          count: 13
           ingredient: {
-            item: "gtceu:steel_nugget"
+            item: "gtceu:wrought_iron_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:annealed_copper_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_lv_bisalloy_400_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 650
+  duration: 850
   inputs: {
     fluid: [
       {
         content: {
-          amount: 650
+          amount: 850
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gcyr:lv_bisalloy_400_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 8
           ingredient: {
             item: "gtceu:steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gcyr:bisalloy_400_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 1
+          count: 2
           ingredient: {
-            item: "gtceu:steel_nugget"
+            item: "gtceu:annealed_copper_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 13
+          ingredient: {
+            item: "gtceu:wrought_iron_nugget"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_lv_bisalloy_400_screwdriver</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 538
+  duration: 1071
   inputs: {
     fluid: [
       {
         content: {
-          amount: 538
+          amount: 1071
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gcyr:lv_bisalloy_400_screwdriver"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tungsten_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "gcyr:bisalloy_400_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:tungsten_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_lv_bisalloy_400_wrench</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 451
+  duration: 658
   inputs: {
     fluid: [
       {
         content: {
-          amount: 451
+          amount: 658
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gcyr:lv_bisalloy_400_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 41
           ingredient: {
             item: "gtceu:steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gcyr:bisalloy_400_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:annealed_copper_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 13
+          ingredient: {
+            item: "gtceu:wrought_iron_nugget"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_lv_blue_steel_chainsaw</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 629
+  duration: 804
   inputs: {
     fluid: [
       {
         content: {
-          amount: 629
+          amount: 804
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_blue_steel_chainsaw"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 8
           ingredient: {
             item: "gtceu:steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 2
           ingredient: {
             item: "gtceu:blue_steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 5
+          count: 13
           ingredient: {
-            item: "gtceu:steel_nugget"
+            item: "gtceu:wrought_iron_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:annealed_copper_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_lv_blue_steel_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 754
+  duration: 954
   inputs: {
     fluid: [
       {
         content: {
-          amount: 754
+          amount: 954
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_blue_steel_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 8
           ingredient: {
             item: "gtceu:steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:blue_steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 1
+          count: 2
           ingredient: {
-            item: "gtceu:steel_nugget"
+            item: "gtceu:annealed_copper_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 13
+          ingredient: {
+            item: "gtceu:wrought_iron_nugget"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_lv_blue_steel_wrench</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 555
+  duration: 762
   inputs: {
     fluid: [
       {
         content: {
-          amount: 555
+          amount: 762
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_blue_steel_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 41
           ingredient: {
             item: "gtceu:steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:blue_steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:annealed_copper_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 13
+          ingredient: {
+            item: "gtceu:wrought_iron_nugget"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_lv_bronze_chainsaw</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 631
+  duration: 806
   inputs: {
     fluid: [
       {
         content: {
-          amount: 631
+          amount: 806
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_bronze_chainsaw"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 8
           ingredient: {
             item: "gtceu:steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 2
           ingredient: {
             item: "gtceu:bronze_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 5
+          count: 13
           ingredient: {
-            item: "gtceu:steel_nugget"
+            item: "gtceu:wrought_iron_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:annealed_copper_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_lv_bronze_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 758
+  duration: 958
   inputs: {
     fluid: [
       {
         content: {
-          amount: 758
+          amount: 958
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_bronze_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 8
           ingredient: {
             item: "gtceu:steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:bronze_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 1
+          count: 2
           ingredient: {
-            item: "gtceu:steel_nugget"
+            item: "gtceu:annealed_copper_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 13
+          ingredient: {
+            item: "gtceu:wrought_iron_nugget"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_lv_bronze_screwdriver</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 565
+  duration: 1098
   inputs: {
     fluid: [
       {
         content: {
-          amount: 565
+          amount: 1098
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_bronze_screwdriver"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tungsten_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "gtceu:bronze_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:tungsten_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_lv_bronze_wrench</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 559
+  duration: 766
   inputs: {
     fluid: [
       {
         content: {
-          amount: 559
+          amount: 766
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_bronze_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 41
           ingredient: {
             item: "gtceu:steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:bronze_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:annealed_copper_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 13
+          ingredient: {
+            item: "gtceu:wrought_iron_nugget"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_lv_cobalt_brass_chainsaw</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 595
+  duration: 770
   inputs: {
     fluid: [
       {
         content: {
-          amount: 595
+          amount: 770
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_cobalt_brass_chainsaw"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 8
           ingredient: {
             item: "gtceu:steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 2
           ingredient: {
             item: "gtceu:cobalt_brass_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 5
+          count: 13
           ingredient: {
-            item: "gtceu:steel_nugget"
+            item: "gtceu:wrought_iron_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:annealed_copper_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_lv_cobalt_brass_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 686
+  duration: 886
   inputs: {
     fluid: [
       {
         content: {
-          amount: 686
+          amount: 886
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_cobalt_brass_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 8
           ingredient: {
             item: "gtceu:steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:cobalt_brass_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 1
+          count: 2
           ingredient: {
-            item: "gtceu:steel_nugget"
+            item: "gtceu:annealed_copper_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 13
+          ingredient: {
+            item: "gtceu:wrought_iron_nugget"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_lv_cobalt_brass_screwdriver</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 547
+  duration: 1080
   inputs: {
     fluid: [
       {
         content: {
-          amount: 547
+          amount: 1080
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_cobalt_brass_screwdriver"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tungsten_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "gtceu:cobalt_brass_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:tungsten_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_lv_cobalt_brass_wrench</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 487
+  duration: 694
   inputs: {
     fluid: [
       {
         content: {
-          amount: 487
+          amount: 694
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_cobalt_brass_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 41
           ingredient: {
             item: "gtceu:steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:cobalt_brass_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:annealed_copper_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 13
+          ingredient: {
+            item: "gtceu:wrought_iron_nugget"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_lv_damascus_steel_chainsaw</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 591
+  duration: 766
   inputs: {
     fluid: [
       {
         content: {
-          amount: 591
+          amount: 766
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_damascus_steel_chainsaw"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 8
           ingredient: {
             item: "gtceu:steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 2
           ingredient: {
             item: "gtceu:damascus_steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 5
+          count: 13
           ingredient: {
-            item: "gtceu:steel_nugget"
+            item: "gtceu:wrought_iron_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:annealed_copper_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_lv_damascus_steel_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 678
+  duration: 878
   inputs: {
     fluid: [
       {
         content: {
-          amount: 678
+          amount: 878
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_damascus_steel_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 8
           ingredient: {
             item: "gtceu:steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:damascus_steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 1
+          count: 2
           ingredient: {
-            item: "gtceu:steel_nugget"
+            item: "gtceu:annealed_copper_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 13
+          ingredient: {
+            item: "gtceu:wrought_iron_nugget"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_lv_damascus_steel_wrench</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 479
+  duration: 686
   inputs: {
     fluid: [
       {
         content: {
-          amount: 479
+          amount: 686
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_damascus_steel_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 41
           ingredient: {
             item: "gtceu:steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:damascus_steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:annealed_copper_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 13
+          ingredient: {
+            item: "gtceu:wrought_iron_nugget"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_lv_diamond_chainsaw</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 482
+  duration: 772
   inputs: {
     fluid: [
       {
         content: {
-          amount: 482
+          amount: 772
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_diamond_chainsaw"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 8
           ingredient: {
             item: "gtceu:steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 5
+          count: 2
           ingredient: {
-            item: "gtceu:steel_nugget"
+            item: "gtceu:annealed_copper_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
-            item: "gtceu:small_carbon_dust"
+            item: "gtceu:tin_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 13
+          ingredient: {
+            item: "gtceu:wrought_iron_nugget"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_lv_diamond_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 460
+  duration: 772
   inputs: {
     fluid: [
       {
         content: {
-          amount: 460
+          amount: 772
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_diamond_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 8
           ingredient: {
             item: "gtceu:steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
-            item: "gtceu:steel_nugget"
+            item: "gtceu:tin_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 2
           ingredient: {
-            item: "gtceu:small_carbon_dust"
+            item: "gtceu:annealed_copper_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 13
+          ingredient: {
+            item: "gtceu:wrought_iron_nugget"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_lv_diamond_wrench</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 261
+  duration: 580
   inputs: {
     fluid: [
       {
         content: {
-          amount: 261
+          amount: 580
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_diamond_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 41
           ingredient: {
             item: "gtceu:steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 2
           ingredient: {
-            item: "gtceu:small_carbon_dust"
+            item: "gtceu:annealed_copper_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 13
+          ingredient: {
+            item: "gtceu:wrought_iron_nugget"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 1
+          ingredient: {
+            item: "gtceu:tin_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_lv_duranium_chainsaw</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 1079
+  duration: 1254
   inputs: {
     fluid: [
       {
         content: {
-          amount: 1079
+          amount: 1254
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_duranium_chainsaw"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 8
           ingredient: {
             item: "gtceu:steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 2
           ingredient: {
             item: "gtceu:duranium_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 5
+          count: 13
           ingredient: {
-            item: "gtceu:steel_nugget"
+            item: "gtceu:wrought_iron_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:annealed_copper_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_lv_duranium_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 1654
+  duration: 1854
   inputs: {
     fluid: [
       {
         content: {
-          amount: 1654
+          amount: 1854
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_duranium_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 8
           ingredient: {
             item: "gtceu:steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:duranium_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 1
+          count: 2
           ingredient: {
-            item: "gtceu:steel_nugget"
+            item: "gtceu:annealed_copper_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 13
+          ingredient: {
+            item: "gtceu:wrought_iron_nugget"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_lv_duranium_wrench</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 1455
+  duration: 1662
   inputs: {
     fluid: [
       {
         content: {
-          amount: 1455
+          amount: 1662
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_duranium_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 41
           ingredient: {
             item: "gtceu:steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:duranium_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:annealed_copper_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 13
+          ingredient: {
+            item: "gtceu:wrought_iron_nugget"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_lv_hsse_chainsaw</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 641
+  duration: 816
   inputs: {
     fluid: [
       {
         content: {
-          amount: 641
+          amount: 816
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_hsse_chainsaw"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 8
           ingredient: {
             item: "gtceu:steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 2
           ingredient: {
             item: "gtceu:hsse_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 5
+          count: 13
           ingredient: {
-            item: "gtceu:steel_nugget"
+            item: "gtceu:wrought_iron_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:annealed_copper_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_lv_hsse_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 778
+  duration: 978
   inputs: {
     fluid: [
       {
         content: {
-          amount: 778
+          amount: 978
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_hsse_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 8
           ingredient: {
             item: "gtceu:steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:hsse_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 1
+          count: 2
           ingredient: {
-            item: "gtceu:steel_nugget"
+            item: "gtceu:annealed_copper_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 13
+          ingredient: {
+            item: "gtceu:wrought_iron_nugget"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_lv_hsse_screwdriver</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 570
+  duration: 1103
   inputs: {
     fluid: [
       {
         content: {
-          amount: 570
+          amount: 1103
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_hsse_screwdriver"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tungsten_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "gtceu:hsse_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:tungsten_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_lv_hsse_wrench</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 579
+  duration: 786
   inputs: {
     fluid: [
       {
         content: {
-          amount: 579
+          amount: 786
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_hsse_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 41
           ingredient: {
             item: "gtceu:steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:hsse_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:annealed_copper_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 13
+          ingredient: {
+            item: "gtceu:wrought_iron_nugget"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_lv_invar_chainsaw</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 591
+  duration: 766
   inputs: {
     fluid: [
       {
         content: {
-          amount: 591
+          amount: 766
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_invar_chainsaw"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 8
           ingredient: {
             item: "gtceu:steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 2
           ingredient: {
             item: "gtceu:invar_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 5
+          count: 13
           ingredient: {
-            item: "gtceu:steel_nugget"
+            item: "gtceu:wrought_iron_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:annealed_copper_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_lv_invar_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 678
+  duration: 878
   inputs: {
     fluid: [
       {
         content: {
-          amount: 678
+          amount: 878
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_invar_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 8
           ingredient: {
             item: "gtceu:steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:invar_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 1
+          count: 2
           ingredient: {
-            item: "gtceu:steel_nugget"
+            item: "gtceu:annealed_copper_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 13
+          ingredient: {
+            item: "gtceu:wrought_iron_nugget"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_lv_invar_screwdriver</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 545
+  duration: 1078
   inputs: {
     fluid: [
       {
         content: {
-          amount: 545
+          amount: 1078
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_invar_screwdriver"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tungsten_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "gtceu:invar_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:tungsten_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_lv_invar_wrench</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 479
+  duration: 686
   inputs: {
     fluid: [
       {
         content: {
-          amount: 479
+          amount: 686
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_invar_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 41
           ingredient: {
             item: "gtceu:steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:invar_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:annealed_copper_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 13
+          ingredient: {
+            item: "gtceu:wrought_iron_nugget"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_lv_iron_chainsaw</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 591
+  duration: 884
   inputs: {
     fluid: [
       {
         content: {
-          amount: 591
+          amount: 884
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_iron_chainsaw"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 8
           ingredient: {
             item: "gtceu:steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 2
           ingredient: {
-            item: "gtceu:wrought_iron_ingot"
+            item: "gtceu:annealed_copper_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 5
+          count: 1
           ingredient: {
-            item: "gtceu:steel_nugget"
+            item: "gtceu:tin_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 31
+          ingredient: {
+            item: "gtceu:wrought_iron_nugget"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_lv_iron_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 678
+  duration: 996
   inputs: {
     fluid: [
       {
         content: {
-          amount: 678
+          amount: 996
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_iron_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 8
           ingredient: {
             item: "gtceu:steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 4
+          count: 49
           ingredient: {
-            item: "gtceu:wrought_iron_ingot"
+            item: "gtceu:wrought_iron_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
-            item: "gtceu:steel_nugget"
+            item: "gtceu:tin_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:annealed_copper_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_lv_iron_screwdriver</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 545
+  duration: 1078
   inputs: {
     fluid: [
       {
         content: {
-          amount: 545
+          amount: 1078
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_iron_screwdriver"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tungsten_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "gtceu:wrought_iron_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:tungsten_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_lv_iron_wrench</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 479
+  duration: 804
   inputs: {
     fluid: [
       {
         content: {
-          amount: 479
+          amount: 804
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_iron_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 41
           ingredient: {
             item: "gtceu:steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 4
+          count: 2
           ingredient: {
-            item: "gtceu:wrought_iron_ingot"
+            item: "gtceu:annealed_copper_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 49
+          ingredient: {
+            item: "gtceu:wrought_iron_nugget"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 1
+          ingredient: {
+            item: "gtceu:tin_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_lv_naquadah_alloy_chainsaw</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 1261
+  duration: 1436
   inputs: {
     fluid: [
       {
         content: {
-          amount: 1261
+          amount: 1436
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_naquadah_alloy_chainsaw"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 8
           ingredient: {
             item: "gtceu:steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 2
           ingredient: {
             item: "gtceu:naquadah_alloy_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 5
+          count: 13
           ingredient: {
-            item: "gtceu:steel_nugget"
+            item: "gtceu:wrought_iron_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:annealed_copper_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_lv_naquadah_alloy_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 2018
+  duration: 2218
   inputs: {
     fluid: [
       {
         content: {
-          amount: 2018
+          amount: 2218
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_naquadah_alloy_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 8
           ingredient: {
             item: "gtceu:steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:naquadah_alloy_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 1
+          count: 2
           ingredient: {
-            item: "gtceu:steel_nugget"
+            item: "gtceu:annealed_copper_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 13
+          ingredient: {
+            item: "gtceu:wrought_iron_nugget"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_lv_naquadah_alloy_screwdriver</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 880
+  duration: 1413
   inputs: {
     fluid: [
       {
         content: {
-          amount: 880
+          amount: 1413
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_naquadah_alloy_screwdriver"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tungsten_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "gtceu:naquadah_alloy_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:tungsten_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_lv_naquadah_alloy_wrench</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 1819
+  duration: 2026
   inputs: {
     fluid: [
       {
         content: {
-          amount: 1819
+          amount: 2026
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_naquadah_alloy_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 41
           ingredient: {
             item: "gtceu:steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:naquadah_alloy_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:annealed_copper_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 13
+          ingredient: {
+            item: "gtceu:wrought_iron_nugget"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_lv_neutronium_chainsaw</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 2479
+  duration: 2654
   inputs: {
     fluid: [
       {
         content: {
-          amount: 2479
+          amount: 2654
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_neutronium_chainsaw"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 8
           ingredient: {
             item: "gtceu:steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 2
           ingredient: {
             item: "gtceu:neutronium_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 5
+          count: 13
           ingredient: {
-            item: "gtceu:steel_nugget"
+            item: "gtceu:wrought_iron_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:annealed_copper_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_lv_neutronium_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 4454
+  duration: 4654
   inputs: {
     fluid: [
       {
         content: {
-          amount: 4454
+          amount: 4654
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_neutronium_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 8
           ingredient: {
             item: "gtceu:steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:neutronium_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 1
+          count: 2
           ingredient: {
-            item: "gtceu:steel_nugget"
+            item: "gtceu:annealed_copper_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 13
+          ingredient: {
+            item: "gtceu:wrought_iron_nugget"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_lv_neutronium_wrench</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 4255
+  duration: 4462
   inputs: {
     fluid: [
       {
         content: {
-          amount: 4255
+          amount: 4462
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_neutronium_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 41
           ingredient: {
             item: "gtceu:steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:neutronium_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:annealed_copper_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 13
+          ingredient: {
+            item: "gtceu:wrought_iron_nugget"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_lv_red_steel_chainsaw</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 617
+  duration: 792
   inputs: {
     fluid: [
       {
         content: {
-          amount: 617
+          amount: 792
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_red_steel_chainsaw"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 8
           ingredient: {
             item: "gtceu:steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 2
           ingredient: {
             item: "gtceu:red_steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 5
+          count: 13
           ingredient: {
-            item: "gtceu:steel_nugget"
+            item: "gtceu:wrought_iron_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:annealed_copper_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_lv_red_steel_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 730
+  duration: 930
   inputs: {
     fluid: [
       {
         content: {
-          amount: 730
+          amount: 930
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_red_steel_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 8
           ingredient: {
             item: "gtceu:steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:red_steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 1
+          count: 2
           ingredient: {
-            item: "gtceu:steel_nugget"
+            item: "gtceu:annealed_copper_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 13
+          ingredient: {
+            item: "gtceu:wrought_iron_nugget"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_lv_red_steel_wrench</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 531
+  duration: 738
   inputs: {
     fluid: [
       {
         content: {
-          amount: 531
+          amount: 738
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_red_steel_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 41
           ingredient: {
             item: "gtceu:steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:red_steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:annealed_copper_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 13
+          ingredient: {
+            item: "gtceu:wrought_iron_nugget"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_lv_rose_gold_chainsaw</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 817
+  duration: 992
   inputs: {
     fluid: [
       {
         content: {
-          amount: 817
+          amount: 992
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_rose_gold_chainsaw"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 8
           ingredient: {
             item: "gtceu:steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 2
           ingredient: {
             item: "gtceu:rose_gold_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 5
+          count: 13
           ingredient: {
-            item: "gtceu:steel_nugget"
+            item: "gtceu:wrought_iron_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:annealed_copper_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_lv_rose_gold_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 1130
+  duration: 1330
   inputs: {
     fluid: [
       {
         content: {
-          amount: 1130
+          amount: 1330
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_rose_gold_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 8
           ingredient: {
             item: "gtceu:steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:rose_gold_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 1
+          count: 2
           ingredient: {
-            item: "gtceu:steel_nugget"
+            item: "gtceu:annealed_copper_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 13
+          ingredient: {
+            item: "gtceu:wrought_iron_nugget"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_lv_rose_gold_screwdriver</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 658
+  duration: 1191
   inputs: {
     fluid: [
       {
         content: {
-          amount: 658
+          amount: 1191
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_rose_gold_screwdriver"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tungsten_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "gtceu:rose_gold_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:tungsten_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_lv_rose_gold_wrench</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 931
+  duration: 1138
   inputs: {
     fluid: [
       {
         content: {
-          amount: 931
+          amount: 1138
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_rose_gold_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 41
           ingredient: {
             item: "gtceu:steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:rose_gold_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:annealed_copper_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 13
+          ingredient: {
+            item: "gtceu:wrought_iron_nugget"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_lv_stainless_steel_chainsaw</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 589
+  duration: 764
   inputs: {
     fluid: [
       {
         content: {
-          amount: 589
+          amount: 764
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_stainless_steel_chainsaw"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 8
           ingredient: {
             item: "gtceu:steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 2
           ingredient: {
             item: "firmalife:metal/ingot/stainless_steel"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 5
+          count: 13
           ingredient: {
-            item: "gtceu:steel_nugget"
+            item: "gtceu:wrought_iron_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:annealed_copper_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_lv_stainless_steel_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 674
+  duration: 874
   inputs: {
     fluid: [
       {
         content: {
-          amount: 674
+          amount: 874
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_stainless_steel_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 8
           ingredient: {
             item: "gtceu:steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "firmalife:metal/ingot/stainless_steel"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 1
+          count: 2
           ingredient: {
-            item: "gtceu:steel_nugget"
+            item: "gtceu:annealed_copper_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 13
+          ingredient: {
+            item: "gtceu:wrought_iron_nugget"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_lv_stainless_steel_screwdriver</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 544
+  duration: 1077
   inputs: {
     fluid: [
       {
         content: {
-          amount: 544
+          amount: 1077
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_stainless_steel_screwdriver"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tungsten_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "firmalife:metal/ingot/stainless_steel"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:tungsten_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_lv_stainless_steel_wrench</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 475
+  duration: 682
   inputs: {
     fluid: [
       {
         content: {
-          amount: 475
+          amount: 682
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_stainless_steel_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 41
           ingredient: {
             item: "gtceu:steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "firmalife:metal/ingot/stainless_steel"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:annealed_copper_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 13
+          ingredient: {
+            item: "gtceu:wrought_iron_nugget"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_lv_steel_chainsaw</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 591
+  duration: 798
   inputs: {
     fluid: [
       {
         content: {
-          amount: 591
+          amount: 798
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_steel_chainsaw"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "gtceu:steel_block"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 14
           ingredient: {
             item: "gtceu:steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:annealed_copper_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 13
+          ingredient: {
+            item: "gtceu:wrought_iron_nugget"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_lv_steel_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 678
+  duration: 885
   inputs: {
     fluid: [
       {
         content: {
-          amount: 678
+          amount: 885
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_steel_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "gtceu:steel_block"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 28
           ingredient: {
             item: "gtceu:steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:annealed_copper_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 13
+          ingredient: {
+            item: "gtceu:wrought_iron_nugget"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_lv_steel_screwdriver</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 545
+  duration: 1078
   inputs: {
     fluid: [
       {
         content: {
-          amount: 545
+          amount: 1078
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_steel_screwdriver"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tungsten_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "gtceu:steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:tungsten_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_lv_steel_wrench</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 479
+  duration: 772
   inputs: {
     fluid: [
       {
         content: {
-          amount: 479
+          amount: 772
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_steel_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 8
           ingredient: {
             item: "gtceu:steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 5
+          count: 2
           ingredient: {
-            item: "gtceu:steel_nugget"
+            item: "gtceu:annealed_copper_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 13
+          ingredient: {
+            item: "gtceu:wrought_iron_nugget"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 1
+          ingredient: {
+            item: "gtceu:tin_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_lv_sterling_silver_chainsaw</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 675
+  duration: 850
   inputs: {
     fluid: [
       {
         content: {
-          amount: 675
+          amount: 850
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_sterling_silver_chainsaw"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 8
           ingredient: {
             item: "gtceu:steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 2
           ingredient: {
             item: "gtceu:sterling_silver_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 5
+          count: 13
           ingredient: {
-            item: "gtceu:steel_nugget"
+            item: "gtceu:wrought_iron_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:annealed_copper_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_lv_sterling_silver_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 846
+  duration: 1046
   inputs: {
     fluid: [
       {
         content: {
-          amount: 846
+          amount: 1046
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_sterling_silver_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 8
           ingredient: {
             item: "gtceu:steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:sterling_silver_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 1
+          count: 2
           ingredient: {
-            item: "gtceu:steel_nugget"
+            item: "gtceu:annealed_copper_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 13
+          ingredient: {
+            item: "gtceu:wrought_iron_nugget"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_lv_sterling_silver_screwdriver</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 587
+  duration: 1120
   inputs: {
     fluid: [
       {
         content: {
-          amount: 587
+          amount: 1120
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_sterling_silver_screwdriver"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tungsten_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "gtceu:sterling_silver_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:tungsten_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_lv_sterling_silver_wrench</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 647
+  duration: 854
   inputs: {
     fluid: [
       {
         content: {
-          amount: 647
+          amount: 854
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_sterling_silver_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 41
           ingredient: {
             item: "gtceu:steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:sterling_silver_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:annealed_copper_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 13
+          ingredient: {
+            item: "gtceu:wrought_iron_nugget"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_lv_titanium_chainsaw</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 575
+  duration: 750
   inputs: {
     fluid: [
       {
         content: {
-          amount: 575
+          amount: 750
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_titanium_chainsaw"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 8
           ingredient: {
             item: "gtceu:steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 2
           ingredient: {
             item: "gtceu:titanium_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 5
+          count: 13
           ingredient: {
-            item: "gtceu:steel_nugget"
+            item: "gtceu:wrought_iron_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:annealed_copper_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_lv_titanium_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 646
+  duration: 846
   inputs: {
     fluid: [
       {
         content: {
-          amount: 646
+          amount: 846
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_titanium_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 8
           ingredient: {
             item: "gtceu:steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:titanium_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 1
+          count: 2
           ingredient: {
-            item: "gtceu:steel_nugget"
+            item: "gtceu:annealed_copper_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 13
+          ingredient: {
+            item: "gtceu:wrought_iron_nugget"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_lv_titanium_screwdriver</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 537
+  duration: 1070
   inputs: {
     fluid: [
       {
         content: {
-          amount: 537
+          amount: 1070
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_titanium_screwdriver"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tungsten_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "gtceu:titanium_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:tungsten_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_lv_titanium_wrench</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 447
+  duration: 654
   inputs: {
     fluid: [
       {
         content: {
-          amount: 447
+          amount: 654
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_titanium_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 41
           ingredient: {
             item: "gtceu:steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:titanium_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:annealed_copper_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 13
+          ingredient: {
+            item: "gtceu:wrought_iron_nugget"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_lv_tungsten_carbide_chainsaw</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 673
+  duration: 848
   inputs: {
     fluid: [
       {
         content: {
-          amount: 673
+          amount: 848
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_tungsten_carbide_chainsaw"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 8
           ingredient: {
             item: "gtceu:steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 2
           ingredient: {
             item: "gtceu:tungsten_carbide_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 5
+          count: 13
           ingredient: {
-            item: "gtceu:steel_nugget"
+            item: "gtceu:wrought_iron_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:annealed_copper_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_lv_tungsten_carbide_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 842
+  duration: 1042
   inputs: {
     fluid: [
       {
         content: {
-          amount: 842
+          amount: 1042
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_tungsten_carbide_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 8
           ingredient: {
             item: "gtceu:steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:tungsten_carbide_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 1
+          count: 2
           ingredient: {
-            item: "gtceu:steel_nugget"
+            item: "gtceu:annealed_copper_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 13
+          ingredient: {
+            item: "gtceu:wrought_iron_nugget"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_lv_tungsten_carbide_screwdriver</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 586
+  duration: 1119
   inputs: {
     fluid: [
       {
         content: {
-          amount: 586
+          amount: 1119
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_tungsten_carbide_screwdriver"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tungsten_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "gtceu:tungsten_carbide_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:tungsten_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_lv_tungsten_carbide_wrench</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 643
+  duration: 850
   inputs: {
     fluid: [
       {
         content: {
-          amount: 643
+          amount: 850
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_tungsten_carbide_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 41
           ingredient: {
             item: "gtceu:steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:tungsten_carbide_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:annealed_copper_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 13
+          ingredient: {
+            item: "gtceu:wrought_iron_nugget"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_lv_tungsten_steel_chainsaw</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 717
+  duration: 892
   inputs: {
     fluid: [
       {
         content: {
-          amount: 717
+          amount: 892
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_tungsten_steel_chainsaw"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 8
           ingredient: {
             item: "gtceu:steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 2
           ingredient: {
             item: "gtceu:tungsten_steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 5
+          count: 13
           ingredient: {
-            item: "gtceu:steel_nugget"
+            item: "gtceu:wrought_iron_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:annealed_copper_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_lv_tungsten_steel_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 930
+  duration: 1130
   inputs: {
     fluid: [
       {
         content: {
-          amount: 930
+          amount: 1130
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_tungsten_steel_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 8
           ingredient: {
             item: "gtceu:steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:tungsten_steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 1
+          count: 2
           ingredient: {
-            item: "gtceu:steel_nugget"
+            item: "gtceu:annealed_copper_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 13
+          ingredient: {
+            item: "gtceu:wrought_iron_nugget"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_lv_tungsten_steel_screwdriver</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 608
+  duration: 1205
   inputs: {
     fluid: [
       {
         content: {
-          amount: 608
+          amount: 1205
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_tungsten_steel_screwdriver"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 46
+          count: 55
           ingredient: {
             item: "gtceu:tungsten_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:tungsten_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:neodymium_nugget"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_lv_tungsten_steel_wrench</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 731
+  duration: 938
   inputs: {
     fluid: [
       {
         content: {
-          amount: 731
+          amount: 938
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_tungsten_steel_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 41
           ingredient: {
             item: "gtceu:steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:tungsten_steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:annealed_copper_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 13
+          ingredient: {
+            item: "gtceu:wrought_iron_nugget"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_lv_ultimet_chainsaw</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 601
+  duration: 776
   inputs: {
     fluid: [
       {
         content: {
-          amount: 601
+          amount: 776
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_ultimet_chainsaw"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 8
           ingredient: {
             item: "gtceu:steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 2
           ingredient: {
             item: "gtceu:ultimet_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 5
+          count: 13
           ingredient: {
-            item: "gtceu:steel_nugget"
+            item: "gtceu:wrought_iron_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:annealed_copper_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_lv_ultimet_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 698
+  duration: 898
   inputs: {
     fluid: [
       {
         content: {
-          amount: 698
+          amount: 898
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_ultimet_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 8
           ingredient: {
             item: "gtceu:steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:ultimet_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 1
+          count: 2
           ingredient: {
-            item: "gtceu:steel_nugget"
+            item: "gtceu:annealed_copper_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 13
+          ingredient: {
+            item: "gtceu:wrought_iron_nugget"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_lv_ultimet_screwdriver</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 550
+  duration: 1083
   inputs: {
     fluid: [
       {
         content: {
-          amount: 550
+          amount: 1083
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_ultimet_screwdriver"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tungsten_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "gtceu:ultimet_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:tungsten_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_lv_ultimet_wrench</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 499
+  duration: 706
   inputs: {
     fluid: [
       {
         content: {
-          amount: 499
+          amount: 706
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_ultimet_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 41
           ingredient: {
             item: "gtceu:steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:ultimet_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:annealed_copper_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 13
+          ingredient: {
+            item: "gtceu:wrought_iron_nugget"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_lv_vanadium_steel_chainsaw</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 589
+  duration: 764
   inputs: {
     fluid: [
       {
         content: {
-          amount: 589
+          amount: 764
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_vanadium_steel_chainsaw"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 8
           ingredient: {
             item: "gtceu:steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 2
           ingredient: {
             item: "gtceu:vanadium_steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 5
+          count: 13
           ingredient: {
-            item: "gtceu:steel_nugget"
+            item: "gtceu:wrought_iron_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:annealed_copper_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_lv_vanadium_steel_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 674
+  duration: 874
   inputs: {
     fluid: [
       {
         content: {
-          amount: 674
+          amount: 874
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_vanadium_steel_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 8
           ingredient: {
             item: "gtceu:steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:vanadium_steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 1
+          count: 2
           ingredient: {
-            item: "gtceu:steel_nugget"
+            item: "gtceu:annealed_copper_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 13
+          ingredient: {
+            item: "gtceu:wrought_iron_nugget"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_lv_vanadium_steel_screwdriver</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 544
+  duration: 1077
   inputs: {
     fluid: [
       {
         content: {
-          amount: 544
+          amount: 1077
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_vanadium_steel_screwdriver"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tungsten_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "gtceu:vanadium_steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:tungsten_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_lv_vanadium_steel_wrench</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 475
+  duration: 682
   inputs: {
     fluid: [
       {
         content: {
-          amount: 475
+          amount: 682
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_vanadium_steel_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 41
           ingredient: {
             item: "gtceu:steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:vanadium_steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:annealed_copper_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 13
+          ingredient: {
+            item: "gtceu:wrought_iron_nugget"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_lv_wrought_iron_chainsaw</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 591
+  duration: 884
   inputs: {
     fluid: [
       {
         content: {
-          amount: 591
+          amount: 884
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_wrought_iron_chainsaw"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 8
           ingredient: {
             item: "gtceu:steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 2
           ingredient: {
-            item: "gtceu:wrought_iron_ingot"
+            item: "gtceu:annealed_copper_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 5
+          count: 1
           ingredient: {
-            item: "gtceu:steel_nugget"
+            item: "gtceu:tin_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 31
+          ingredient: {
+            item: "gtceu:wrought_iron_nugget"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_lv_wrought_iron_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 678
+  duration: 996
   inputs: {
     fluid: [
       {
         content: {
-          amount: 678
+          amount: 996
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_wrought_iron_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 8
           ingredient: {
             item: "gtceu:steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 4
+          count: 49
           ingredient: {
-            item: "gtceu:wrought_iron_ingot"
+            item: "gtceu:wrought_iron_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
-            item: "gtceu:steel_nugget"
+            item: "gtceu:tin_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:annealed_copper_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_lv_wrought_iron_screwdriver</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 545
+  duration: 1078
   inputs: {
     fluid: [
       {
         content: {
-          amount: 545
+          amount: 1078
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_wrought_iron_screwdriver"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tungsten_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "gtceu:wrought_iron_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:tungsten_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_lv_wrought_iron_wrench</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 479
+  duration: 804
   inputs: {
     fluid: [
       {
         content: {
-          amount: 479
+          amount: 804
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_wrought_iron_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 41
           ingredient: {
             item: "gtceu:steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 4
+          count: 2
           ingredient: {
-            item: "gtceu:wrought_iron_ingot"
+            item: "gtceu:annealed_copper_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 49
+          ingredient: {
+            item: "gtceu:wrought_iron_nugget"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 1
+          ingredient: {
+            item: "gtceu:tin_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_mv_aluminium_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 434
+  duration: 785
   inputs: {
     fluid: [
       {
         content: {
-          amount: 434
+          amount: 785
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:mv_aluminium_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
-      {
-        content: {
-          type: "gtceu:sized"
-          count: 8
-          ingredient: {
-            item: "gtceu:aluminium_ingot"
-          }
-        }
-        chance: 1
-        tierChanceBoost: 0
-      }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
-            item: "gtceu:steel_ingot"
+            item: "gtceu:cupronickel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
-            item: "gtceu:aluminium_nugget"
+            item: "gtceu:aluminium_block"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 40
+          ingredient: {
+            item: "gtceu:steel_nugget"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 1
+          ingredient: {
+            item: "gtceu:annealed_copper_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_mv_bisalloy_400_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 526
+  duration: 817
   inputs: {
     fluid: [
       {
         content: {
-          amount: 526
+          amount: 817
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gcyr:mv_bisalloy_400_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:aluminium_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 4
+          count: 40
           ingredient: {
-            item: "gtceu:steel_ingot"
+            item: "gtceu:steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gcyr:bisalloy_400_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:cupronickel_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_mv_blue_steel_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 630
+  duration: 921
   inputs: {
     fluid: [
       {
         content: {
-          amount: 630
+          amount: 921
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:mv_blue_steel_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:aluminium_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:blue_steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
-            item: "gtceu:steel_ingot"
+            item: "gtceu:cupronickel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 40
+          ingredient: {
+            item: "gtceu:steel_nugget"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_mv_bronze_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 634
+  duration: 925
   inputs: {
     fluid: [
       {
         content: {
-          amount: 634
+          amount: 925
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:mv_bronze_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:aluminium_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:bronze_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
-            item: "gtceu:steel_ingot"
+            item: "gtceu:cupronickel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 40
+          ingredient: {
+            item: "gtceu:steel_nugget"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_mv_cobalt_brass_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 562
+  duration: 853
   inputs: {
     fluid: [
       {
         content: {
-          amount: 562
+          amount: 853
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:mv_cobalt_brass_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:aluminium_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:cobalt_brass_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
-            item: "gtceu:steel_ingot"
+            item: "gtceu:cupronickel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 40
+          ingredient: {
+            item: "gtceu:steel_nugget"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_mv_damascus_steel_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 554
+  duration: 845
   inputs: {
     fluid: [
       {
         content: {
-          amount: 554
+          amount: 845
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:mv_damascus_steel_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:aluminium_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:damascus_steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
-            item: "gtceu:steel_ingot"
+            item: "gtceu:cupronickel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 40
+          ingredient: {
+            item: "gtceu:steel_nugget"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_mv_diamond_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 336
+  duration: 684
   inputs: {
     fluid: [
       {
         content: {
-          amount: 336
+          amount: 684
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:mv_diamond_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:aluminium_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
-            item: "gtceu:steel_ingot"
+            item: "gtceu:cupronickel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 2
+          count: 1
           ingredient: {
-            item: "gtceu:small_carbon_dust"
+            item: "gtceu:annealed_copper_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 40
+          ingredient: {
+            item: "gtceu:steel_nugget"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_mv_duranium_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 1530
+  duration: 1821
   inputs: {
     fluid: [
       {
         content: {
-          amount: 1530
+          amount: 1821
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:mv_duranium_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:aluminium_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 4
+          count: 40
           ingredient: {
-            item: "gtceu:steel_ingot"
+            item: "gtceu:steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:duranium_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:cupronickel_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_mv_hsse_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 654
+  duration: 945
   inputs: {
     fluid: [
       {
         content: {
-          amount: 654
+          amount: 945
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:mv_hsse_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:aluminium_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 4
+          count: 40
           ingredient: {
-            item: "gtceu:steel_ingot"
+            item: "gtceu:steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:hsse_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:cupronickel_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_mv_invar_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 554
+  duration: 845
   inputs: {
     fluid: [
       {
         content: {
-          amount: 554
+          amount: 845
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:mv_invar_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:aluminium_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:invar_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
-            item: "gtceu:steel_ingot"
+            item: "gtceu:cupronickel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 40
+          ingredient: {
+            item: "gtceu:steel_nugget"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_mv_iron_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 554
+  duration: 845
   inputs: {
     fluid: [
       {
         content: {
-          amount: 554
+          amount: 845
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:mv_iron_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:aluminium_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:wrought_iron_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
-            item: "gtceu:steel_ingot"
+            item: "gtceu:cupronickel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 40
+          ingredient: {
+            item: "gtceu:steel_nugget"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_mv_muffler_hatch</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 799
+  duration: 762
   inputs: {
     fluid: [
       {
         content: {
-          amount: 799
+          amount: 762
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "gtceu:mv_muffler_hatch"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:bronze_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:cupronickel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 31
           ingredient: {
             item: "gtceu:steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
-            item: "gtceu:annealed_copper_ingot"
+            item: "gtceu:aluminium_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_mv_naquadah_alloy_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 1894
+  duration: 2185
   inputs: {
     fluid: [
       {
         content: {
-          amount: 1894
+          amount: 2185
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:mv_naquadah_alloy_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:aluminium_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 4
+          count: 40
           ingredient: {
-            item: "gtceu:steel_ingot"
+            item: "gtceu:steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:naquadah_alloy_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:cupronickel_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_mv_neutronium_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 4330
+  duration: 4621
   inputs: {
     fluid: [
       {
         content: {
-          amount: 4330
+          amount: 4621
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:mv_neutronium_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:aluminium_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 4
+          count: 40
           ingredient: {
-            item: "gtceu:steel_ingot"
+            item: "gtceu:steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:neutronium_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:cupronickel_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_mv_red_steel_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 606
+  duration: 897
   inputs: {
     fluid: [
       {
         content: {
-          amount: 606
+          amount: 897
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:mv_red_steel_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:aluminium_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 4
+          count: 40
           ingredient: {
-            item: "gtceu:steel_ingot"
+            item: "gtceu:steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:red_steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:cupronickel_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_mv_rose_gold_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 1006
+  duration: 1297
   inputs: {
     fluid: [
       {
         content: {
-          amount: 1006
+          amount: 1297
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:mv_rose_gold_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:aluminium_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:rose_gold_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
-            item: "gtceu:steel_ingot"
+            item: "gtceu:cupronickel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 40
+          ingredient: {
+            item: "gtceu:steel_nugget"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_mv_stainless_steel_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 550
+  duration: 841
   inputs: {
     fluid: [
       {
         content: {
-          amount: 550
+          amount: 841
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:mv_stainless_steel_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:aluminium_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 4
+          count: 40
           ingredient: {
-            item: "gtceu:steel_ingot"
+            item: "gtceu:steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "firmalife:metal/ingot/stainless_steel"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:cupronickel_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_mv_steel_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 554
+  duration: 883
   inputs: {
     fluid: [
       {
         content: {
-          amount: 554
+          amount: 883
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:mv_steel_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 8
           ingredient: {
             item: "gtceu:steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:aluminium_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:cupronickel_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 1
+          ingredient: {
+            item: "gtceu:annealed_copper_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_mv_sterling_silver_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 722
+  duration: 1013
   inputs: {
     fluid: [
       {
         content: {
-          amount: 722
+          amount: 1013
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:mv_sterling_silver_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:aluminium_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 4
+          count: 40
           ingredient: {
-            item: "gtceu:steel_ingot"
+            item: "gtceu:steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:sterling_silver_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:cupronickel_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_mv_titanium_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 522
+  duration: 813
   inputs: {
     fluid: [
       {
         content: {
-          amount: 522
+          amount: 813
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:mv_titanium_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:aluminium_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:titanium_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
-            item: "gtceu:steel_ingot"
+            item: "gtceu:cupronickel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 40
+          ingredient: {
+            item: "gtceu:steel_nugget"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_mv_tungsten_carbide_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 718
+  duration: 1009
   inputs: {
     fluid: [
       {
         content: {
-          amount: 718
+          amount: 1009
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:mv_tungsten_carbide_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:aluminium_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 4
+          count: 40
           ingredient: {
-            item: "gtceu:steel_ingot"
+            item: "gtceu:steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:tungsten_carbide_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:cupronickel_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_mv_tungsten_steel_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 806
+  duration: 1097
   inputs: {
     fluid: [
       {
         content: {
-          amount: 806
+          amount: 1097
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:mv_tungsten_steel_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:aluminium_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 4
+          count: 40
           ingredient: {
-            item: "gtceu:steel_ingot"
+            item: "gtceu:steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:tungsten_steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:cupronickel_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_mv_ultimet_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 574
+  duration: 865
   inputs: {
     fluid: [
       {
         content: {
-          amount: 574
+          amount: 865
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:mv_ultimet_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:aluminium_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:ultimet_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
-            item: "gtceu:steel_ingot"
+            item: "gtceu:cupronickel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 40
+          ingredient: {
+            item: "gtceu:steel_nugget"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_mv_vanadium_steel_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 550
+  duration: 841
   inputs: {
     fluid: [
       {
         content: {
-          amount: 550
+          amount: 841
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:mv_vanadium_steel_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:aluminium_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 4
+          count: 40
           ingredient: {
-            item: "gtceu:steel_ingot"
+            item: "gtceu:steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:vanadium_steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:cupronickel_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_mv_wrought_iron_drill</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 554
+  duration: 845
   inputs: {
     fluid: [
       {
         content: {
-          amount: 554
+          amount: 845
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:mv_wrought_iron_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:aluminium_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:wrought_iron_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
-            item: "gtceu:steel_ingot"
+            item: "gtceu:cupronickel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 40
+          ingredient: {
+            item: "gtceu:steel_nugget"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_naquadah_alloy_buzzsaw</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 2053
+  duration: 2586
   inputs: {
     fluid: [
       {
         content: {
-          amount: 2053
+          amount: 2586
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:naquadah_alloy_buzzsaw"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tungsten_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:naquadah_alloy_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:tungsten_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_neutronium_buzzsaw</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 4489
+  duration: 5022
   inputs: {
     fluid: [
       {
         content: {
-          amount: 4489
+          amount: 5022
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:neutronium_buzzsaw"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tungsten_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:neutronium_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:tungsten_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_red_steel_buzzsaw</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 765
+  duration: 1298
   inputs: {
     fluid: [
       {
         content: {
-          amount: 765
+          amount: 1298
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:red_steel_buzzsaw"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tungsten_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:red_steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:tungsten_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_rose_gold_buzzsaw</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 1165
+  duration: 1698
   inputs: {
     fluid: [
       {
         content: {
-          amount: 1165
+          amount: 1698
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:rose_gold_buzzsaw"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tungsten_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:rose_gold_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:tungsten_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_stainless_steel_buzzsaw</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 709
+  duration: 1242
   inputs: {
     fluid: [
       {
         content: {
-          amount: 709
+          amount: 1242
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:stainless_steel_buzzsaw"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tungsten_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "firmalife:metal/ingot/stainless_steel"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:tungsten_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_steel_buzzsaw</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 713
+  duration: 1246
   inputs: {
     fluid: [
       {
         content: {
-          amount: 713
+          amount: 1246
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:steel_buzzsaw"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tungsten_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:tungsten_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_sterling_silver_buzzsaw</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 881
+  duration: 1414
   inputs: {
     fluid: [
       {
         content: {
-          amount: 881
+          amount: 1414
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:sterling_silver_buzzsaw"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tungsten_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:sterling_silver_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:tungsten_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_titanium_buzzsaw</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 681
+  duration: 1214
   inputs: {
     fluid: [
       {
         content: {
-          amount: 681
+          amount: 1214
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:titanium_buzzsaw"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tungsten_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:titanium_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:tungsten_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_tungsten_carbide_buzzsaw</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 877
+  duration: 1410
   inputs: {
     fluid: [
       {
         content: {
-          amount: 877
+          amount: 1410
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:tungsten_carbide_buzzsaw"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tungsten_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:tungsten_carbide_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:tungsten_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_tungsten_steel_buzzsaw</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 965
+  duration: 1549
   inputs: {
     fluid: [
       {
         content: {
-          amount: 965
+          amount: 1549
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:tungsten_steel_buzzsaw"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
-      {
-        content: {
-          type: "gtceu:sized"
-          count: 8
-          ingredient: {
-            item: "gtceu:tungsten_steel_ingot"
-          }
-        }
-        chance: 1
-        tierChanceBoost: 0
-      }
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
-            item: "gtceu:tungsten_steel_nugget"
+            item: "gtceu:tungsten_steel_block"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:tungsten_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:neodymium_nugget"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_ultimet_buzzsaw</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 733
+  duration: 1266
   inputs: {
     fluid: [
       {
         content: {
-          amount: 733
+          amount: 1266
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:ultimet_buzzsaw"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tungsten_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:ultimet_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:tungsten_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_vanadium_steel_buzzsaw</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 709
+  duration: 1242
   inputs: {
     fluid: [
       {
         content: {
-          amount: 709
+          amount: 1242
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:vanadium_steel_buzzsaw"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tungsten_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:vanadium_steel_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:tungsten_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/arc_furnace/arc_wrought_iron_buzzsaw</summary>

```diff
 {
   type: "gtceu:arc_furnace"
-  duration: 713
+  duration: 1246
   inputs: {
     fluid: [
       {
         content: {
-          amount: 713
+          amount: 1246
           value: [
             {
               tag: "forge:oxygen"
             }
           ]
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:wrought_iron_buzzsaw"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tungsten_steel_nugget"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:wrought_iron_ingot"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:tungsten_ingot"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/forge_hammer/loose_andesite</summary>

```diff
 {
   type: "gtceu:forge_hammer"
-  duration: 120
+  duration: 60
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "tfc:rock/raw/andesite"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "tfc:rock/loose/andesite"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
 }

```


</details>

<details>
<summary>gtceu/forge_hammer/loose_basalt</summary>

```diff
 {
   type: "gtceu:forge_hammer"
-  duration: 120
+  duration: 60
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "tfc:rock/raw/basalt"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "tfc:rock/loose/basalt"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
 }

```


</details>

<details>
<summary>gtceu/forge_hammer/loose_chalk</summary>

```diff
 {
   type: "gtceu:forge_hammer"
-  duration: 120
+  duration: 60
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "tfc:rock/raw/chalk"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "tfc:rock/loose/chalk"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
 }

```


</details>

<details>
<summary>gtceu/forge_hammer/loose_chert</summary>

```diff
 {
   type: "gtceu:forge_hammer"
-  duration: 120
+  duration: 60
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "tfc:rock/raw/chert"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "tfc:rock/loose/chert"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
 }

```


</details>

<details>
<summary>gtceu/forge_hammer/loose_claystone</summary>

```diff
 {
   type: "gtceu:forge_hammer"
-  duration: 120
+  duration: 60
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "tfc:rock/raw/claystone"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "tfc:rock/loose/claystone"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
 }

```


</details>

<details>
<summary>gtceu/forge_hammer/loose_conglomerate</summary>

```diff
 {
   type: "gtceu:forge_hammer"
-  duration: 120
+  duration: 60
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "tfc:rock/raw/conglomerate"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "tfc:rock/loose/conglomerate"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
 }

```


</details>

<details>
<summary>gtceu/forge_hammer/loose_dacite</summary>

```diff
 {
   type: "gtceu:forge_hammer"
-  duration: 120
+  duration: 60
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "tfc:rock/raw/dacite"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "tfc:rock/loose/dacite"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
 }

```


</details>

<details>
<summary>gtceu/forge_hammer/loose_diorite</summary>

```diff
 {
   type: "gtceu:forge_hammer"
-  duration: 120
+  duration: 60
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "tfc:rock/raw/diorite"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "tfc:rock/loose/diorite"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
 }

```


</details>

<details>
<summary>gtceu/forge_hammer/loose_dolomite</summary>

```diff
 {
   type: "gtceu:forge_hammer"
-  duration: 120
+  duration: 60
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "tfc:rock/raw/dolomite"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "tfc:rock/loose/dolomite"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
 }

```


</details>

<details>
<summary>gtceu/forge_hammer/loose_gabbro</summary>

```diff
 {
   type: "gtceu:forge_hammer"
-  duration: 120
+  duration: 60
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "tfc:rock/raw/gabbro"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "tfc:rock/loose/gabbro"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
 }

```


</details>

<details>
<summary>gtceu/forge_hammer/loose_gneiss</summary>

```diff
 {
   type: "gtceu:forge_hammer"
-  duration: 120
+  duration: 60
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "tfc:rock/raw/gneiss"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "tfc:rock/loose/gneiss"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
 }

```


</details>

<details>
<summary>gtceu/forge_hammer/loose_granite</summary>

```diff
 {
   type: "gtceu:forge_hammer"
-  duration: 120
+  duration: 60
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "tfc:rock/raw/granite"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "tfc:rock/loose/granite"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
 }

```


</details>

<details>
<summary>gtceu/forge_hammer/loose_limestone</summary>

```diff
 {
   type: "gtceu:forge_hammer"
-  duration: 120
+  duration: 60
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "tfc:rock/raw/limestone"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "tfc:rock/loose/limestone"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
 }

```


</details>

<details>
<summary>gtceu/forge_hammer/loose_marble</summary>

```diff
 {
   type: "gtceu:forge_hammer"
-  duration: 120
+  duration: 60
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "tfc:rock/raw/marble"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "tfc:rock/loose/marble"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
 }

```


</details>

<details>
<summary>gtceu/forge_hammer/loose_phyllite</summary>

```diff
 {
   type: "gtceu:forge_hammer"
-  duration: 120
+  duration: 60
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "tfc:rock/raw/phyllite"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "tfc:rock/loose/phyllite"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
 }

```


</details>

<details>
<summary>gtceu/forge_hammer/loose_quartzite</summary>

```diff
 {
   type: "gtceu:forge_hammer"
-  duration: 120
+  duration: 60
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "tfc:rock/raw/quartzite"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "tfc:rock/loose/quartzite"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
 }

```


</details>

<details>
<summary>gtceu/forge_hammer/loose_rhyolite</summary>

```diff
 {
   type: "gtceu:forge_hammer"
-  duration: 120
+  duration: 60
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "tfc:rock/raw/rhyolite"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "tfc:rock/loose/rhyolite"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
 }

```


</details>

<details>
<summary>gtceu/forge_hammer/loose_schist</summary>

```diff
 {
   type: "gtceu:forge_hammer"
-  duration: 120
+  duration: 60
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "tfc:rock/raw/schist"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "tfc:rock/loose/schist"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
 }

```


</details>

<details>
<summary>gtceu/forge_hammer/loose_shale</summary>

```diff
 {
   type: "gtceu:forge_hammer"
-  duration: 120
+  duration: 60
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "tfc:rock/raw/shale"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "tfc:rock/loose/shale"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
 }

```


</details>

<details>
<summary>gtceu/forge_hammer/loose_slate</summary>

```diff
 {
   type: "gtceu:forge_hammer"
-  duration: 120
+  duration: 60
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "tfc:rock/raw/slate"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 30
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "tfc:rock/loose/slate"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_aluminium_buzzsaw</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 593
+  duration: 1126
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:aluminium_buzzsaw"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_tungsten_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:aluminium_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:tungsten_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 32
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_basalt</summary>

```diff
 {
   type: "gtceu:macerator"
   duration: 150
   inputs: {
     item: [
       {
         content: {
-          children: [
-            {
-              tag: "forge:basalt"
-            }
-            {
-              tag: "forge:stone"
-            }
-          ]
+          count: 1
+          ingredient: {
+            item: "minecraft:basalt"
+          }
-          type: "forge:intersection"
+          type: "gtceu:sized"
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "gtceu:basalt_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "gtceu:basalt_dust"
           }
         }
         chance: 0.1
         tierChanceBoost: 0.038
       }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 2
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_bisalloy_400_buzzsaw</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 685
+  duration: 1218
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gcyr:bisalloy_400_buzzsaw"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_tungsten_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gcyr:bisalloy_400_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:tungsten_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 32
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_blue_steel_buzzsaw</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 789
+  duration: 1322
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:blue_steel_buzzsaw"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_tungsten_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:blue_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:tungsten_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 32
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_bronze_buzzsaw</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 793
+  duration: 1326
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:bronze_buzzsaw"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_tungsten_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:bronze_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:tungsten_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 32
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_cobalt_brass_buzzsaw</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 721
+  duration: 1254
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:cobalt_brass_buzzsaw"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_tungsten_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:cobalt_brass_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:tungsten_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 32
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_damascus_steel_buzzsaw</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 713
+  duration: 1246
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:damascus_steel_buzzsaw"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_tungsten_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:damascus_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:tungsten_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 32
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_diamond_buzzsaw</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 537
+  duration: 1070
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:diamond_buzzsaw"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_tungsten_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:diamond_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:tungsten_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 32
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_diamond_lens</summary>

```diff
 {
   type: "gtceu:macerator"
   duration: 9
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
-            tag: "forge:lenses/light_blue"
+            tag: "forge:lenses/diamond"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 3
           ingredient: {
             item: "gtceu:small_diamond_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 2
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_diorite</summary>

```diff
 {
   type: "gtceu:macerator"
   duration: 150
   inputs: {
     item: [
       {
         content: {
-          children: [
-            {
-              tag: "forge:diorite"
-            }
-            {
-              tag: "forge:stone"
-            }
-          ]
+          count: 1
+          ingredient: {
+            item: "minecraft:diorite"
+          }
-          type: "forge:intersection"
+          type: "gtceu:sized"
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "gtceu:diorite_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
-            item: "gtceu:small_stone_dust"
+            item: "gtceu:stone_dust"
           }
         }
-        chance: 0.01
+        chance: 0.001
-        tierChanceBoost: 0.004
+        tierChanceBoost: 0.0005
       }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 2
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_duranium_buzzsaw</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 1689
+  duration: 2222
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:duranium_buzzsaw"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_tungsten_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:duranium_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:tungsten_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 32
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_ev_aluminium_drill</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 525
+  duration: 801
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:ev_aluminium_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_titanium_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 4
+          count: 6
           ingredient: {
             item: "gtceu:aluminium_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:kanthal_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 8
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_ev_bisalloy_400_drill</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 617
+  duration: 841
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gcyr:ev_bisalloy_400_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_titanium_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gcyr:bisalloy_400_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:kanthal_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 32
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_ev_block_breaker</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 960
+  duration: 890
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "gtceu:ev_block_breaker"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 8
           ingredient: {
             item: "gtceu:steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 8
           ingredient: {
             item: "gtceu:kanthal_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 6
           ingredient: {
             item: "gtceu:rubber_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 5
           ingredient: {
-            item: "gtceu:aluminium_dust"
+            item: "gtceu:diamond_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 8
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_ev_blue_steel_drill</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 721
+  duration: 945
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:ev_blue_steel_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_titanium_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:blue_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:kanthal_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 8
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_ev_bronze_drill</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 725
+  duration: 949
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:ev_bronze_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_titanium_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:bronze_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:kanthal_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 8
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_ev_cobalt_brass_drill</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 653
+  duration: 877
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:ev_cobalt_brass_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_titanium_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:cobalt_brass_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:kanthal_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 8
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_ev_damascus_steel_drill</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 645
+  duration: 869
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:ev_damascus_steel_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_titanium_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:damascus_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:kanthal_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 8
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_ev_diamond_drill</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 469
+  duration: 693
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:ev_diamond_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_titanium_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:diamond_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:kanthal_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 8
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_ev_duranium_drill</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 1621
+  duration: 1845
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:ev_duranium_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_titanium_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:duranium_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:kanthal_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 8
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_ev_hsse_drill</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 745
+  duration: 969
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:ev_hsse_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_titanium_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:hsse_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:kanthal_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 32
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_ev_invar_drill</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 645
+  duration: 869
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:ev_invar_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_titanium_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:invar_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:kanthal_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 8
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_ev_iron_drill</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 645
+  duration: 869
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:ev_iron_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_titanium_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:iron_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:kanthal_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 8
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_ev_naquadah_alloy_drill</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 1985
+  duration: 2209
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:ev_naquadah_alloy_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_titanium_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:naquadah_alloy_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:kanthal_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 32
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_ev_neutronium_drill</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 4421
+  duration: 4645
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:ev_neutronium_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_titanium_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:neutronium_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:kanthal_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 8
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_ev_red_steel_drill</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 697
+  duration: 921
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:ev_red_steel_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_titanium_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:red_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:kanthal_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 8
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_ev_rose_gold_drill</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 1097
+  duration: 1321
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:ev_rose_gold_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_titanium_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:rose_gold_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:kanthal_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 8
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_ev_stainless_steel_drill</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 641
+  duration: 865
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:ev_stainless_steel_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_titanium_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:stainless_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:kanthal_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 8
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_ev_steel_drill</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 645
+  duration: 921
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:ev_steel_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 8
           ingredient: {
             item: "gtceu:steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_titanium_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:kanthal_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:aluminium_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 8
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_ev_sterling_silver_drill</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 813
+  duration: 1037
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:ev_sterling_silver_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_titanium_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:sterling_silver_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:kanthal_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 8
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_ev_titanium_drill</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 608
+  duration: 884
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:ev_titanium_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 32
+          count: 36
           ingredient: {
             item: "gtceu:small_titanium_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:kanthal_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:aluminium_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 8
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_ev_tungsten_carbide_drill</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 809
+  duration: 1033
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:ev_tungsten_carbide_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_titanium_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:tungsten_carbide_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:kanthal_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 32
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_ev_tungsten_steel_drill</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 897
+  duration: 1121
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:ev_tungsten_steel_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_titanium_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:tungsten_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:kanthal_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 32
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_ev_ultimet_drill</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 665
+  duration: 889
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:ev_ultimet_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_titanium_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:ultimet_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:kanthal_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 32
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_ev_vanadium_steel_drill</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 641
+  duration: 865
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:ev_vanadium_steel_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_titanium_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:vanadium_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:kanthal_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 8
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_ev_wrought_iron_drill</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 645
+  duration: 869
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:ev_wrought_iron_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_titanium_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:wrought_iron_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:kanthal_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 8
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_glass_lens</summary>

```diff
 {
   type: "gtceu:macerator"
   duration: 15
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
-            tag: "forge:lenses/white"
+            tag: "forge:lenses/glass"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 3
           ingredient: {
             item: "gtceu:small_glass_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 2
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_granite</summary>

```diff
 {
   type: "gtceu:macerator"
   duration: 150
   inputs: {
     item: [
       {
         content: {
-          children: [
-            {
-              tag: "forge:granite"
-            }
-            {
-              tag: "forge:stone"
-            }
-          ]
+          count: 1
+          ingredient: {
+            item: "minecraft:granite"
+          }
-          type: "forge:intersection"
+          type: "gtceu:sized"
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "gtceu:granite_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
-            item: "gtceu:small_stone_dust"
+            item: "gtceu:stone_dust"
           }
         }
-        chance: 0.01
+        chance: 0.001
-        tierChanceBoost: 0.004
+        tierChanceBoost: 0.0005
       }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 2
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_hp_steam_extractor</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 1631
+  duration: 1667
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "gtceu:hp_steam_extractor"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 14
           ingredient: {
             item: "gtceu:bronze_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 5
           ingredient: {
             item: "gtceu:tin_alloy_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 2
           ingredient: {
             item: "gtceu:wrought_iron_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
-            item: "gtceu:glass_dust"
+            item: "gtceu:steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 8
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_hsse_buzzsaw</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 813
+  duration: 1346
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:hsse_buzzsaw"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_tungsten_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:hsse_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:tungsten_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 32
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_hv_aluminium_drill</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 554
+  duration: 1213
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:hv_aluminium_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_stainless_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:aluminium_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:electrum_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 8
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_hv_aluminium_wrench</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 355
+  duration: 1203
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:hv_aluminium_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_stainless_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:aluminium_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 4
+          count: 2
           ingredient: {
-            item: "gtceu:tiny_steel_dust"
+            item: "gtceu:silver_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:electrum_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 8
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_hv_bisalloy_400_drill</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 646
+  duration: 1305
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gcyr:hv_bisalloy_400_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_stainless_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gcyr:bisalloy_400_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:electrum_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 32
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_hv_bisalloy_400_wrench</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 447
+  duration: 1295
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gcyr:hv_bisalloy_400_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_stainless_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gcyr:bisalloy_400_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 4
+          count: 2
           ingredient: {
-            item: "gtceu:tiny_steel_dust"
+            item: "gtceu:silver_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:electrum_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 32
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_hv_blue_steel_drill</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 750
+  duration: 1409
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:hv_blue_steel_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_stainless_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:blue_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:electrum_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 8
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_hv_blue_steel_wrench</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 551
+  duration: 1399
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:hv_blue_steel_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_stainless_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:blue_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 4
+          count: 2
           ingredient: {
-            item: "gtceu:tiny_steel_dust"
+            item: "gtceu:silver_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:electrum_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 8
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_hv_bronze_drill</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 754
+  duration: 1413
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:hv_bronze_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_stainless_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:bronze_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:electrum_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 8
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_hv_bronze_wrench</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 555
+  duration: 1403
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:hv_bronze_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_stainless_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:bronze_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 4
+          count: 2
           ingredient: {
-            item: "gtceu:tiny_steel_dust"
+            item: "gtceu:silver_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:electrum_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 8
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_hv_cobalt_brass_drill</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 682
+  duration: 1341
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:hv_cobalt_brass_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_stainless_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:cobalt_brass_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:electrum_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 8
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_hv_cobalt_brass_wrench</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 483
+  duration: 1331
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:hv_cobalt_brass_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_stainless_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:cobalt_brass_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 4
+          count: 2
           ingredient: {
-            item: "gtceu:tiny_steel_dust"
+            item: "gtceu:silver_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:electrum_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 8
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_hv_damascus_steel_drill</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 674
+  duration: 1333
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:hv_damascus_steel_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_stainless_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:damascus_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:electrum_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 8
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_hv_damascus_steel_wrench</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 475
+  duration: 1323
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:hv_damascus_steel_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_stainless_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:damascus_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
-            item: "gtceu:tiny_steel_dust"
+            item: "gtceu:electrum_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:silver_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 8
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_hv_diamond_drill</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 498
+  duration: 1157
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:hv_diamond_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_stainless_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:diamond_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:electrum_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 8
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_hv_diamond_wrench</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 299
+  duration: 1147
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:hv_diamond_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_stainless_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:diamond_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 4
+          count: 2
           ingredient: {
-            item: "gtceu:tiny_steel_dust"
+            item: "gtceu:silver_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:electrum_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 8
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_hv_duranium_drill</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 1650
+  duration: 2309
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:hv_duranium_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_stainless_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:duranium_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:electrum_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 8
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_hv_duranium_wrench</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 1451
+  duration: 2299
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:hv_duranium_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_stainless_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:duranium_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 4
+          count: 2
           ingredient: {
-            item: "gtceu:tiny_steel_dust"
+            item: "gtceu:silver_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:electrum_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 8
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_hv_forming_press</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 2356
+  duration: 2712
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "gtceu:hv_forming_press"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 12
           ingredient: {
             item: "gtceu:stainless_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 12
           ingredient: {
             item: "gtceu:rubber_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 8
           ingredient: {
             item: "gtceu:electrum_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
-            item: "gtceu:silver_dust"
+            item: "gtceu:gold_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 8
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_hv_hsse_drill</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 774
+  duration: 1433
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:hv_hsse_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_stainless_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:hsse_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:electrum_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 32
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_hv_hsse_wrench</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 575
+  duration: 1423
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:hv_hsse_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_stainless_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:hsse_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 4
+          count: 2
           ingredient: {
-            item: "gtceu:tiny_steel_dust"
+            item: "gtceu:silver_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:electrum_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 32
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_hv_invar_drill</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 674
+  duration: 1333
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:hv_invar_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_stainless_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:invar_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:electrum_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 8
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_hv_invar_wrench</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 475
+  duration: 1323
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:hv_invar_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_stainless_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:invar_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 4
+          count: 2
           ingredient: {
-            item: "gtceu:tiny_steel_dust"
+            item: "gtceu:silver_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:electrum_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 8
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_hv_iron_drill</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 674
+  duration: 1333
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:hv_iron_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_stainless_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:iron_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:electrum_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 8
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_hv_iron_wrench</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 475
+  duration: 1323
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:hv_iron_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_stainless_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:iron_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 4
+          count: 2
           ingredient: {
-            item: "gtceu:tiny_steel_dust"
+            item: "gtceu:silver_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:electrum_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 8
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_hv_item_passthrough_hatch</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 1801
+  duration: 1803
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "gtceu:hv_item_passthrough_hatch"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 11
           ingredient: {
             item: "gtceu:rubber_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 8
           ingredient: {
             item: "gtceu:electrum_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:silver_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 2
           ingredient: {
-            item: "gtceu:stainless_steel_dust"
+            item: "gtceu:steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 8
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_hv_laser_engraver</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 2356
+  duration: 2712
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "gtceu:hv_laser_engraver"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 12
           ingredient: {
             item: "gtceu:stainless_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 12
           ingredient: {
             item: "gtceu:rubber_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 8
           ingredient: {
             item: "gtceu:electrum_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
-            item: "gtceu:silver_dust"
+            item: "gtceu:gold_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 8
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_hv_naquadah_alloy_drill</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 2014
+  duration: 2673
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:hv_naquadah_alloy_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_stainless_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:naquadah_alloy_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:electrum_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 32
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_hv_naquadah_alloy_wrench</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 1815
+  duration: 2663
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:hv_naquadah_alloy_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_stainless_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:naquadah_alloy_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 4
+          count: 2
           ingredient: {
-            item: "gtceu:tiny_steel_dust"
+            item: "gtceu:silver_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:electrum_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 32
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_hv_neutronium_drill</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 4450
+  duration: 5109
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:hv_neutronium_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_stainless_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:neutronium_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:electrum_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 8
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_hv_neutronium_wrench</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 4251
+  duration: 5099
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:hv_neutronium_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_stainless_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:neutronium_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
-            item: "gtceu:tiny_steel_dust"
+            item: "gtceu:electrum_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:silver_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 8
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_hv_red_steel_drill</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 726
+  duration: 1385
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:hv_red_steel_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_stainless_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:red_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:electrum_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 8
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_hv_red_steel_wrench</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 527
+  duration: 1375
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:hv_red_steel_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_stainless_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:red_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 4
+          count: 2
           ingredient: {
-            item: "gtceu:tiny_steel_dust"
+            item: "gtceu:silver_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:electrum_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 8
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_hv_rose_gold_drill</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 1126
+  duration: 1785
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:hv_rose_gold_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_stainless_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:rose_gold_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:electrum_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 8
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_hv_rose_gold_wrench</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 927
+  duration: 1775
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:hv_rose_gold_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_stainless_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:rose_gold_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 4
+          count: 2
           ingredient: {
-            item: "gtceu:tiny_steel_dust"
+            item: "gtceu:silver_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:electrum_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 8
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_hv_sifter</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 2346
+  duration: 2178
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "gtceu:hv_sifter"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 12
           ingredient: {
             item: "gtceu:stainless_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 10
           ingredient: {
             item: "gtceu:rubber_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 8
           ingredient: {
             item: "gtceu:electrum_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
-            item: "gtceu:silver_dust"
+            item: "gtceu:zinc_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 8
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_hv_stainless_steel_drill</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 664
+  duration: 1537
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:hv_stainless_steel_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 32
+          count: 36
           ingredient: {
             item: "gtceu:small_stainless_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:electrum_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:silver_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 8
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_hv_stainless_steel_wrench</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 464
+  duration: 1323
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:hv_stainless_steel_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 32
+          count: 36
           ingredient: {
             item: "gtceu:small_stainless_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
-            item: "gtceu:tiny_steel_dust"
+            item: "gtceu:electrum_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:silver_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:rubber_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 8
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_hv_steel_drill</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 674
+  duration: 1547
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:hv_steel_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 8
           ingredient: {
             item: "gtceu:steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_stainless_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:electrum_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:silver_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 8
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_hv_steel_wrench</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 475
+  duration: 1348
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:hv_steel_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 40
           ingredient: {
             item: "gtceu:tiny_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_stainless_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:electrum_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:silver_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 8
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_hv_sterling_silver_drill</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 842
+  duration: 1501
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:hv_sterling_silver_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_stainless_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:sterling_silver_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:electrum_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 8
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_hv_sterling_silver_wrench</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 643
+  duration: 1491
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:hv_sterling_silver_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_stainless_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:sterling_silver_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 4
+          count: 2
           ingredient: {
-            item: "gtceu:tiny_steel_dust"
+            item: "gtceu:silver_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:electrum_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 8
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_hv_titanium_drill</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 642
+  duration: 1301
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:hv_titanium_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_stainless_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:titanium_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:electrum_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 8
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_hv_titanium_wrench</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 443
+  duration: 1291
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:hv_titanium_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_stainless_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:titanium_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 4
+          count: 2
           ingredient: {
-            item: "gtceu:tiny_steel_dust"
+            item: "gtceu:silver_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:electrum_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 8
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_hv_tungsten_carbide_drill</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 838
+  duration: 1497
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:hv_tungsten_carbide_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_stainless_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:tungsten_carbide_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:electrum_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 32
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_hv_tungsten_carbide_wrench</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 639
+  duration: 1487
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:hv_tungsten_carbide_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_stainless_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:tungsten_carbide_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 4
+          count: 2
           ingredient: {
-            item: "gtceu:tiny_steel_dust"
+            item: "gtceu:silver_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:electrum_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 32
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_hv_tungsten_steel_drill</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 926
+  duration: 1585
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:hv_tungsten_steel_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_stainless_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:tungsten_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:electrum_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 32
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_hv_tungsten_steel_wrench</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 727
+  duration: 1575
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:hv_tungsten_steel_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_stainless_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:tungsten_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 4
+          count: 2
           ingredient: {
-            item: "gtceu:tiny_steel_dust"
+            item: "gtceu:silver_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:electrum_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 32
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_hv_ultimet_drill</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 694
+  duration: 1353
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:hv_ultimet_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_stainless_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:ultimet_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:electrum_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 32
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_hv_ultimet_wrench</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 495
+  duration: 1343
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:hv_ultimet_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_stainless_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:ultimet_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 4
+          count: 2
           ingredient: {
-            item: "gtceu:tiny_steel_dust"
+            item: "gtceu:silver_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:electrum_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 32
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_hv_vanadium_steel_drill</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 670
+  duration: 1329
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:hv_vanadium_steel_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_stainless_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:vanadium_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:electrum_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 8
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_hv_vanadium_steel_wrench</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 471
+  duration: 1319
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:hv_vanadium_steel_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_stainless_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:vanadium_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 4
+          count: 2
           ingredient: {
-            item: "gtceu:tiny_steel_dust"
+            item: "gtceu:silver_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:electrum_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 8
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_hv_wrought_iron_drill</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 674
+  duration: 1333
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:hv_wrought_iron_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_stainless_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:wrought_iron_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:electrum_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 8
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_hv_wrought_iron_wrench</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 475
+  duration: 1323
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:hv_wrought_iron_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_stainless_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:wrought_iron_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
-            item: "gtceu:tiny_steel_dust"
+            item: "gtceu:electrum_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:silver_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 8
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_invar_buzzsaw</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 713
+  duration: 1246
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:invar_buzzsaw"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_tungsten_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:invar_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:tungsten_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 32
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_iron_buzzsaw</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 713
+  duration: 1246
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:iron_buzzsaw"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_tungsten_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:iron_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:tungsten_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 32
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_iv_aluminium_drill</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 817
+  duration: 984
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:iv_aluminium_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_tungsten_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:aluminium_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 32
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_iv_aluminium_wrench</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 618
+  duration: 1126
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:iv_aluminium_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_tungsten_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:aluminium_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
-            item: "gtceu:tiny_steel_dust"
+            item: "gtceu:graphene_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:tungsten_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 32
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_iv_bisalloy_400_drill</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 909
+  duration: 1076
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gcyr:iv_bisalloy_400_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_tungsten_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gcyr:bisalloy_400_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 32
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_iv_bisalloy_400_wrench</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 710
+  duration: 1218
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gcyr:iv_bisalloy_400_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_tungsten_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gcyr:bisalloy_400_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
-            item: "gtceu:tiny_steel_dust"
+            item: "gtceu:graphene_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:tungsten_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 32
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_iv_blue_steel_drill</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 1013
+  duration: 1180
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:iv_blue_steel_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_tungsten_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:blue_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 32
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_iv_blue_steel_wrench</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 814
+  duration: 1322
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:iv_blue_steel_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_tungsten_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:blue_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
-            item: "gtceu:tiny_steel_dust"
+            item: "gtceu:graphene_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:tungsten_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 32
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_iv_bronze_drill</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 1017
+  duration: 1184
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:iv_bronze_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_tungsten_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:bronze_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 32
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_iv_bronze_wrench</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 818
+  duration: 1326
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:iv_bronze_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_tungsten_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:bronze_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
-            item: "gtceu:tiny_steel_dust"
+            item: "gtceu:graphene_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:tungsten_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 32
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_iv_cobalt_brass_drill</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 945
+  duration: 1112
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:iv_cobalt_brass_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_tungsten_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:cobalt_brass_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 32
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_iv_cobalt_brass_wrench</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 746
+  duration: 1254
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:iv_cobalt_brass_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_tungsten_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:cobalt_brass_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
-            item: "gtceu:tiny_steel_dust"
+            item: "gtceu:graphene_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:tungsten_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 32
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_iv_damascus_steel_drill</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 937
+  duration: 1104
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:iv_damascus_steel_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_tungsten_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:damascus_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 32
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_iv_damascus_steel_wrench</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 738
+  duration: 1246
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:iv_damascus_steel_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_tungsten_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:damascus_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
-            item: "gtceu:tiny_steel_dust"
+            item: "gtceu:graphene_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:tungsten_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 32
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_iv_diamond_drill</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 761
+  duration: 928
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:iv_diamond_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_tungsten_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:diamond_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 32
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_iv_diamond_wrench</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 562
+  duration: 1070
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:iv_diamond_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_tungsten_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:diamond_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 4
+          count: 2
           ingredient: {
-            item: "gtceu:tiny_steel_dust"
+            item: "gtceu:tungsten_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 32
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_iv_duranium_drill</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 1913
+  duration: 2080
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:iv_duranium_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_tungsten_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:duranium_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 32
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_iv_duranium_wrench</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 1714
+  duration: 2222
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:iv_duranium_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_tungsten_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:duranium_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
-            item: "gtceu:tiny_steel_dust"
+            item: "gtceu:graphene_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:tungsten_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 32
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_iv_hsse_drill</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 1037
+  duration: 1204
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:iv_hsse_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_tungsten_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:hsse_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 32
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_iv_hsse_wrench</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 838
+  duration: 1346
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:iv_hsse_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_tungsten_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:hsse_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
-            item: "gtceu:tiny_steel_dust"
+            item: "gtceu:graphene_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:tungsten_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 32
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_iv_invar_drill</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 937
+  duration: 1104
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:iv_invar_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_tungsten_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:invar_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 32
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_iv_invar_wrench</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 738
+  duration: 1246
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:iv_invar_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_tungsten_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:invar_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
-            item: "gtceu:tiny_steel_dust"
+            item: "gtceu:graphene_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:tungsten_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 32
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_iv_iron_drill</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 937
+  duration: 1104
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:iv_iron_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_tungsten_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:iron_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 32
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_iv_iron_wrench</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 738
+  duration: 1246
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:iv_iron_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_tungsten_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:iron_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 4
+          count: 2
           ingredient: {
-            item: "gtceu:tiny_steel_dust"
+            item: "gtceu:tungsten_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 32
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_iv_naquadah_alloy_drill</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 2277
+  duration: 2444
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:iv_naquadah_alloy_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_tungsten_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:naquadah_alloy_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 32
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_iv_naquadah_alloy_wrench</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 2078
+  duration: 2586
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:iv_naquadah_alloy_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_tungsten_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:naquadah_alloy_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
-            item: "gtceu:tiny_steel_dust"
+            item: "gtceu:graphene_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:tungsten_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 32
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_iv_neutronium_drill</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 4713
+  duration: 4880
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:iv_neutronium_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_tungsten_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:neutronium_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 32
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_iv_neutronium_wrench</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 4514
+  duration: 5022
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:iv_neutronium_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_tungsten_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:neutronium_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
-            item: "gtceu:tiny_steel_dust"
+            item: "gtceu:graphene_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:tungsten_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 32
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_iv_red_steel_drill</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 989
+  duration: 1156
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:iv_red_steel_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_tungsten_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:red_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 32
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_iv_red_steel_wrench</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 790
+  duration: 1298
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:iv_red_steel_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_tungsten_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:red_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 4
+          count: 2
           ingredient: {
-            item: "gtceu:tiny_steel_dust"
+            item: "gtceu:tungsten_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 32
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_iv_rose_gold_drill</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 1389
+  duration: 1556
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:iv_rose_gold_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_tungsten_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:rose_gold_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 32
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_iv_rose_gold_wrench</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 1190
+  duration: 1698
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:iv_rose_gold_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_tungsten_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:rose_gold_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
-            item: "gtceu:tiny_steel_dust"
+            item: "gtceu:graphene_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:tungsten_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 32
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_iv_stainless_steel_drill</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 933
+  duration: 1100
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:iv_stainless_steel_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_tungsten_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:stainless_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 32
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_iv_stainless_steel_wrench</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 734
+  duration: 1242
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:iv_stainless_steel_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_tungsten_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:stainless_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
-            item: "gtceu:tiny_steel_dust"
+            item: "gtceu:graphene_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:tungsten_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 32
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_iv_steel_drill</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 937
+  duration: 1470
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:iv_steel_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 8
           ingredient: {
             item: "gtceu:steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_tungsten_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:tungsten_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 32
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_iv_steel_wrench</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 738
+  duration: 1271
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:iv_steel_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 40
           ingredient: {
             item: "gtceu:tiny_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_tungsten_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:tungsten_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 32
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_iv_sterling_silver_drill</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 1105
+  duration: 1272
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:iv_sterling_silver_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_tungsten_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:sterling_silver_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 32
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_iv_sterling_silver_wrench</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 906
+  duration: 1414
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:iv_sterling_silver_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_tungsten_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:sterling_silver_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
-            item: "gtceu:tiny_steel_dust"
+            item: "gtceu:graphene_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:tungsten_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 32
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_iv_titanium_drill</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 905
+  duration: 1072
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:iv_titanium_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_tungsten_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:titanium_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 32
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_iv_titanium_wrench</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 706
+  duration: 1214
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:iv_titanium_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_tungsten_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:titanium_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
-            item: "gtceu:tiny_steel_dust"
+            item: "gtceu:graphene_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:tungsten_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 32
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_iv_tungsten_carbide_drill</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 1101
+  duration: 1268
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:iv_tungsten_carbide_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_tungsten_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:tungsten_carbide_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 32
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_iv_tungsten_carbide_wrench</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 902
+  duration: 1410
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:iv_tungsten_carbide_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_tungsten_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:tungsten_carbide_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 4
+          count: 2
           ingredient: {
-            item: "gtceu:tiny_steel_dust"
+            item: "gtceu:tungsten_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 32
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_iv_tungsten_steel_drill</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 1176
+  duration: 1709
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:iv_tungsten_steel_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 32
+          count: 36
           ingredient: {
             item: "gtceu:small_tungsten_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:tungsten_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 32
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_iv_tungsten_steel_wrench</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 976
+  duration: 1495
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:iv_tungsten_steel_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 32
+          count: 36
           ingredient: {
             item: "gtceu:small_tungsten_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
-            item: "gtceu:tiny_steel_dust"
+            item: "gtceu:graphene_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:tungsten_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:rubber_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 32
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_iv_ultimet_drill</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 957
+  duration: 1124
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:iv_ultimet_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_tungsten_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:ultimet_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 32
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_iv_ultimet_wrench</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 758
+  duration: 1266
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:iv_ultimet_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_tungsten_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:ultimet_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
-            item: "gtceu:tiny_steel_dust"
+            item: "gtceu:graphene_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:tungsten_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 32
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_iv_vanadium_steel_drill</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 933
+  duration: 1100
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:iv_vanadium_steel_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_tungsten_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:vanadium_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 32
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_iv_vanadium_steel_wrench</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 734
+  duration: 1242
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:iv_vanadium_steel_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_tungsten_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:vanadium_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
-            item: "gtceu:tiny_steel_dust"
+            item: "gtceu:graphene_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:tungsten_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 32
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_iv_wrought_iron_drill</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 937
+  duration: 1104
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:iv_wrought_iron_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_tungsten_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:wrought_iron_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 4
+          ingredient: {
+            item: "gtceu:graphene_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 32
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_iv_wrought_iron_wrench</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 738
+  duration: 1246
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:iv_wrought_iron_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_tungsten_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:wrought_iron_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
-            item: "gtceu:tiny_steel_dust"
+            item: "gtceu:graphene_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:tungsten_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 32
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_lv_aluminium_chainsaw</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 528
+  duration: 664
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_aluminium_chainsaw"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 34
           ingredient: {
             item: "gtceu:small_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 2
           ingredient: {
             item: "gtceu:aluminium_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:copper_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:rubber_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 8
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_lv_aluminium_drill</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 552
+  duration: 688
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_aluminium_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 32
           ingredient: {
             item: "gtceu:small_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:aluminium_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:copper_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:rubber_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 8
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_lv_aluminium_screwdriver</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 515
+  duration: 1032
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_aluminium_screwdriver"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_tungsten_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 1
+          count: 4
           ingredient: {
-            item: "gtceu:aluminium_dust"
+            item: "gtceu:graphene_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:tungsten_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:rubber_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 32
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_lv_aluminium_wrench</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 359
+  duration: 495
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_aluminium_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 41
           ingredient: {
             item: "gtceu:tiny_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:aluminium_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:copper_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:rubber_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 8
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_lv_bisalloy_400_chainsaw</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 574
+  duration: 710
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gcyr:lv_bisalloy_400_chainsaw"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 34
           ingredient: {
             item: "gtceu:small_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 2
           ingredient: {
             item: "gcyr:bisalloy_400_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:copper_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:rubber_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 32
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_lv_bisalloy_400_drill</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 644
+  duration: 780
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gcyr:lv_bisalloy_400_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 32
           ingredient: {
             item: "gtceu:small_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gcyr:bisalloy_400_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:copper_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:rubber_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 32
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_lv_bisalloy_400_screwdriver</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 538
+  duration: 1032
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gcyr:lv_bisalloy_400_screwdriver"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_tungsten_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 1
+          count: 4
           ingredient: {
-            item: "gcyr:bisalloy_400_dust"
+            item: "gtceu:graphene_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:tungsten_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:rubber_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 32
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_lv_bisalloy_400_wrench</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 451
+  duration: 587
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gcyr:lv_bisalloy_400_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 41
           ingredient: {
             item: "gtceu:tiny_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gcyr:bisalloy_400_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:copper_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:rubber_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 32
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_lv_blue_steel_chainsaw</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 626
+  duration: 762
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_blue_steel_chainsaw"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 34
           ingredient: {
             item: "gtceu:small_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 2
           ingredient: {
             item: "gtceu:blue_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:copper_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:rubber_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 8
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_lv_blue_steel_drill</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 748
+  duration: 884
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_blue_steel_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 32
           ingredient: {
             item: "gtceu:small_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:blue_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:copper_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:rubber_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 8
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_lv_blue_steel_wrench</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 555
+  duration: 691
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_blue_steel_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 41
           ingredient: {
             item: "gtceu:tiny_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:blue_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:copper_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:rubber_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 8
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_lv_bronze_chainsaw</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 628
+  duration: 764
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_bronze_chainsaw"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 34
           ingredient: {
             item: "gtceu:small_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 2
           ingredient: {
             item: "gtceu:bronze_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:copper_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:rubber_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 8
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_lv_bronze_drill</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 752
+  duration: 888
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_bronze_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 32
           ingredient: {
             item: "gtceu:small_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:bronze_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:copper_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:rubber_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 8
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_lv_bronze_screwdriver</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 565
+  duration: 1032
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_bronze_screwdriver"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_tungsten_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 1
+          count: 4
           ingredient: {
-            item: "gtceu:bronze_dust"
+            item: "gtceu:graphene_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:tungsten_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:rubber_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 32
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_lv_bronze_wrench</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 559
+  duration: 695
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_bronze_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 41
           ingredient: {
             item: "gtceu:tiny_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:bronze_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:copper_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:rubber_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 8
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_lv_cobalt_brass_chainsaw</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 592
+  duration: 728
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_cobalt_brass_chainsaw"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 34
           ingredient: {
             item: "gtceu:small_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 2
           ingredient: {
             item: "gtceu:cobalt_brass_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:copper_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:rubber_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 8
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_lv_cobalt_brass_drill</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 680
+  duration: 816
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_cobalt_brass_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 32
           ingredient: {
             item: "gtceu:small_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:cobalt_brass_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:copper_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:rubber_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 8
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_lv_cobalt_brass_screwdriver</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 547
+  duration: 1032
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_cobalt_brass_screwdriver"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_tungsten_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 1
+          count: 4
           ingredient: {
-            item: "gtceu:cobalt_brass_dust"
+            item: "gtceu:graphene_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:tungsten_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:rubber_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 32
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_lv_cobalt_brass_wrench</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 487
+  duration: 623
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_cobalt_brass_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 41
           ingredient: {
             item: "gtceu:tiny_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:cobalt_brass_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:copper_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:rubber_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 8
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_lv_damascus_steel_chainsaw</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 588
+  duration: 724
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_damascus_steel_chainsaw"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 34
           ingredient: {
             item: "gtceu:small_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 2
           ingredient: {
             item: "gtceu:damascus_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:copper_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:rubber_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 8
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_lv_damascus_steel_drill</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 672
+  duration: 808
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_damascus_steel_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 32
           ingredient: {
             item: "gtceu:small_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:damascus_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:copper_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:rubber_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 8
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_lv_damascus_steel_wrench</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 479
+  duration: 615
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_damascus_steel_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 41
           ingredient: {
             item: "gtceu:tiny_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:damascus_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:copper_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:rubber_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 8
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_lv_diamond_chainsaw</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 500
+  duration: 636
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_diamond_chainsaw"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 34
           ingredient: {
             item: "gtceu:small_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 2
           ingredient: {
             item: "gtceu:diamond_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:copper_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:rubber_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 8
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_lv_diamond_drill</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 496
+  duration: 632
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_diamond_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 32
           ingredient: {
             item: "gtceu:small_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:diamond_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:copper_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:rubber_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 8
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_lv_diamond_wrench</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 303
+  duration: 439
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_diamond_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 41
           ingredient: {
             item: "gtceu:tiny_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:diamond_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:copper_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:rubber_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 8
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_lv_duranium_chainsaw</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 1076
+  duration: 1212
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_duranium_chainsaw"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 34
           ingredient: {
             item: "gtceu:small_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 2
           ingredient: {
             item: "gtceu:duranium_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:copper_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:rubber_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 8
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_lv_duranium_drill</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 1648
+  duration: 1784
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_duranium_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 32
           ingredient: {
             item: "gtceu:small_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:duranium_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:copper_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:rubber_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 8
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_lv_duranium_wrench</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 1455
+  duration: 1591
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_duranium_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 41
           ingredient: {
             item: "gtceu:tiny_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:duranium_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:copper_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:rubber_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 8
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_lv_hsse_chainsaw</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 638
+  duration: 774
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_hsse_chainsaw"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 34
           ingredient: {
             item: "gtceu:small_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 2
           ingredient: {
             item: "gtceu:hsse_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:copper_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:rubber_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 32
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_lv_hsse_drill</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 772
+  duration: 908
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_hsse_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 32
           ingredient: {
             item: "gtceu:small_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:hsse_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:copper_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:rubber_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 32
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_lv_hsse_screwdriver</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 570
+  duration: 1032
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_hsse_screwdriver"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_tungsten_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 1
+          count: 4
           ingredient: {
-            item: "gtceu:hsse_dust"
+            item: "gtceu:graphene_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:tungsten_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:rubber_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 32
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_lv_hsse_wrench</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 579
+  duration: 715
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_hsse_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 41
           ingredient: {
             item: "gtceu:tiny_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:hsse_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:copper_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:rubber_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 32
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_lv_invar_chainsaw</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 588
+  duration: 724
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_invar_chainsaw"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 34
           ingredient: {
             item: "gtceu:small_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 2
           ingredient: {
             item: "gtceu:invar_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:copper_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:rubber_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 8
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_lv_invar_drill</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 672
+  duration: 808
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_invar_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 32
           ingredient: {
             item: "gtceu:small_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:invar_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:copper_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:rubber_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 8
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_lv_invar_screwdriver</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 545
+  duration: 1032
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_invar_screwdriver"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_tungsten_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 1
+          count: 4
           ingredient: {
-            item: "gtceu:invar_dust"
+            item: "gtceu:graphene_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:tungsten_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:rubber_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 32
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_lv_invar_wrench</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 479
+  duration: 615
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_invar_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 41
           ingredient: {
             item: "gtceu:tiny_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:invar_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:copper_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:rubber_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 8
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_lv_iron_chainsaw</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 588
+  duration: 780
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_iron_chainsaw"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 34
           ingredient: {
             item: "gtceu:small_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 2
+          count: 3
           ingredient: {
             item: "gtceu:iron_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:copper_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:rubber_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 8
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_lv_iron_drill</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 672
+  duration: 864
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_iron_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 32
           ingredient: {
             item: "gtceu:small_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 4
+          count: 5
           ingredient: {
             item: "gtceu:iron_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:copper_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:rubber_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 8
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_lv_iron_screwdriver</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 545
+  duration: 1032
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_iron_screwdriver"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_tungsten_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 1
+          count: 4
           ingredient: {
-            item: "gtceu:iron_dust"
+            item: "gtceu:graphene_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:tungsten_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:rubber_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 32
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_lv_iron_wrench</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 479
+  duration: 671
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_iron_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 41
           ingredient: {
             item: "gtceu:tiny_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 4
+          count: 5
           ingredient: {
             item: "gtceu:iron_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:copper_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:rubber_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 8
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_lv_naquadah_alloy_chainsaw</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 1258
+  duration: 1394
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_naquadah_alloy_chainsaw"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 34
           ingredient: {
             item: "gtceu:small_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 2
           ingredient: {
             item: "gtceu:naquadah_alloy_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:copper_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:rubber_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 32
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_lv_naquadah_alloy_drill</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 2012
+  duration: 2148
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_naquadah_alloy_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 32
           ingredient: {
             item: "gtceu:small_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:naquadah_alloy_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:copper_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:rubber_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 32
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_lv_naquadah_alloy_screwdriver</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 880
+  duration: 1032
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_naquadah_alloy_screwdriver"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
-          count: 37
+          count: 46
           ingredient: {
             item: "gtceu:tiny_tungsten_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
-          count: 1
+          count: 4
           ingredient: {
-            item: "gtceu:naquadah_alloy_dust"
+            item: "gtceu:graphene_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:tungsten_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:rubber_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 32
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_lv_naquadah_alloy_wrench</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 1819
+  duration: 1955
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_naquadah_alloy_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 41
           ingredient: {
             item: "gtceu:tiny_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:naquadah_alloy_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:copper_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:rubber_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 32
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_lv_neutronium_chainsaw</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 2476
+  duration: 2612
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_neutronium_chainsaw"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 34
           ingredient: {
             item: "gtceu:small_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 2
           ingredient: {
             item: "gtceu:neutronium_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:copper_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:rubber_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 8
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_lv_neutronium_drill</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 4448
+  duration: 4584
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_neutronium_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 32
           ingredient: {
             item: "gtceu:small_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:neutronium_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:copper_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:rubber_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 8
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_lv_neutronium_wrench</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 4255
+  duration: 4391
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_neutronium_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 41
           ingredient: {
             item: "gtceu:tiny_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:neutronium_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:copper_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:rubber_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 8
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_lv_power_unit</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 484
+  duration: 422
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             item: "gtceu:lv_power_unit"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 37
           ingredient: {
             item: "gtceu:tiny_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 2
           ingredient: {
             item: "gtceu:copper_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 2
           ingredient: {
             item: "gtceu:rubber_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
-            item: "gtceu:tin_dust"
+            item: "gtceu:iron_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 8
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_lv_red_steel_chainsaw</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 614
+  duration: 750
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_red_steel_chainsaw"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 34
           ingredient: {
             item: "gtceu:small_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 2
           ingredient: {
             item: "gtceu:red_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:copper_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:rubber_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 8
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_lv_red_steel_drill</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 724
+  duration: 860
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_red_steel_drill"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 32
           ingredient: {
             item: "gtceu:small_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:red_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:copper_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:rubber_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 8
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_lv_red_steel_wrench</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 531
+  duration: 667
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_red_steel_wrench"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 41
           ingredient: {
             item: "gtceu:tiny_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 4
           ingredient: {
             item: "gtceu:red_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:copper_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:rubber_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
     ]
   }
   tickInputs: {
     eu: [
       {
         content: 8
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   tickOutputs: {
   }
 }

```


</details>

<details>
<summary>gtceu/macerator/macerate_lv_rose_gold_chainsaw</summary>

```diff
 {
   type: "gtceu:macerator"
-  duration: 814
+  duration: 950
   inputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 1
           ingredient: {
             type: "forge:nbt"
             item: "gtceu:lv_rose_gold_chainsaw"
             count: 1
             nbt: "{GT.Tool:{Damage:0}}"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
     ]
   }
   outputs: {
     item: [
       {
         content: {
           type: "gtceu:sized"
           count: 34
           ingredient: {
             item: "gtceu:small_steel_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
       {
         content: {
           type: "gtceu:sized"
           count: 2
           ingredient: {
             item: "gtceu:rose_gold_dust"
           }
         }
         chance: 1
         tierChanceBoost: 0
       }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:copper_dust"
+          }
+        }
+        chance: 1
+        tierChanceBoost: 0
+      }
+      {
+        content: {
+          type: "gtceu:sized"
+          count: 2
+          ingredient: {
+            item: "gtceu:rubber_dust"
+          }
 }