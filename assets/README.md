# Asset Structure — Dark Survivors

Иерархия ассетов построена по игровым сущностям. Все пути относительны `public/assets/`.

## Текущие ассеты (имеются)

```
ui/
├── coins_hud.png              — иконка золота в HUD
└── skull.png                  — иконка счётчика убийств

pickups/
├── coin.png                   — монета
├── heal.png                   — лечение
└── xp_gem.png                 — кристалл опыта

enemies/dark_forest/basic/
├── goblin.png                 — базовый враг (гоблин) [переименовать из monster_basic]
└── goblin_hit.png             — гоблин при попадании [из monster_basic_hit]
```

## Требуются (создавать по мере необходимости)

### UI
```
ui/
├── merge_btn.png              — кнопка открытия мержа
├── rune_slot.png              — слот инвентаря рун
├── pause.png                  — иконка паузы
├── diamond.png                — иконка Telegram Stars / премиум
└── heart.png                  — иконка HP
```

### Pickups
```
pickups/
├── xp_small.png               — XP (малый)
├── xp_medium.png              — XP (средний)
├── xp_large.png               — XP (большой)
├── xp_huge.png                — XP (огромный, с боссов)
├── food_meat.png              — мясо (+20 HP)
├── food_chicken.png           — курица (+50 HP)
├── gold_bag.png               — мешок золота
├── chest_wooden.png           — деревянный сундук
├── chest_golden.png           — золотой сундук
└── magnet.png                 — магнит (притягивает всё XP)
```

### Runes (4 стихии × 5 рангов)
```
runes/fire/          rank1.png rank2.png rank3.png rank4.png rank5.png
runes/ice/           rank1.png rank2.png rank3.png rank4.png rank5.png
runes/lightning/     rank1.png rank2.png rank3.png rank4.png rank5.png
runes/dark/          rank1.png rank2.png rank3.png rank4.png rank5.png

runes/combined/
├── steam.png                  — Пар (Огонь+Лёд)
├── storm.png                  — Шторм (Огонь+Молния)
├── ash.png                    — Пепел (Огонь+Тьма)
├── frost.png                  — Иней (Лёд+Молния)
├── permafrost.png             — Вечная мерзлота (Лёд+Тьма)
├── abyss.png                  — Бездна (Молния+Тьма)
├── apocalypse.png             — Апокалипсис (тройной)
├── absolute_zero.png          — Абсолютный ноль
├── phoenix.png                — Феникс
└── chaos.png                  — Хаос
```

### Enemies (по биомам)
```
enemies/dark_forest/basic/
├── goblin.png (+ _hit.png)    ✓ ЕСТЬ
├── wolf.png (+ _hit.png)
├── skeleton.png (+ _hit.png)
├── bat.png (+ _hit.png)
├── ent.png (+ _hit.png)       — древент
└── ghost.png (+ _hit.png)

enemies/ice_wastes/
├── ice_slime.png
├── snow_wolf.png
├── ice_golem.png
├── frost_fae.png
└── yeti.png                   (мини-босс)

enemies/volcanic/
├── fire_elemental.png
├── lava_worm.png
├── fire_drake.png
├── magma_golem.png
└── phoenix_spawner.png

enemies/storm_citadel/
├── electro_slime.png
├── thunder_guard.png
├── ball_lightning.png
├── tesla_construct.png
└── storm_dragon.png           (мини-босс)

enemies/<biome>/elite/
└── <base_name>_elite.png      — элитные версии (аура, размер)
```

### Bosses
```
bosses/
├── mushroom_king.png          (Тёмный лес, 5 мин)
├── ice_queen.png              (Ледяные пустоши)
├── volcanic_titan.png
├── storm_lord.png
└── reaper.png                 (финальный, Жнец)
```

### Weapons (иконки для UI выбора при уровне)
```
weapons/
├── throwing_knife.png         (W01)
├── ice_wave.png               (W02)
├── chain_lightning.png        (W03)
├── dark_orb.png               (W04)
├── stone_ring.png             (W05)
├── air_blade.png              (W06)
├── fire_vortex.png            (W07)
├── poison_cloud.png           (W08)
├── holy_beam.png              (W09)
├── shadow_strike.png          (W10)
├── ice_spikes.png             (W11)
├── ball_lightning.png         (W12)
├── bone_spear.png             (W13)
├── fireballs.png              (W14)
└── ice_barrier.png            (W15)
```

### Projectiles (игровые снаряды)
```
projectiles/
├── orb_player.png             — базовый орб (текущий)
├── knife.png
├── ice_shard.png
├── lightning_bolt.png
├── fireball.png
├── bone_spear.png
├── enemy_bullet.png           — красный вражеский снаряд (текущий ShooterEnemy)
└── holy_beam.png
```

### Passives (иконки для выбора при уровне)
```
passives/
├── cloak.png                  (P01 Плащ)
├── ice_heart.png              (P02)
├── capacitor.png              (P03)
├── shadow_book.png            (P04)
├── earth_shield.png           (P05)
├── wind_feather.png           (P06)
├── volcano_heart.png          (P07)
├── alchemist_flask.png        (P08)
├── holy_cross.png             (P09)
├── dark_amulet.png            (P10)
├── snowflake.png              (P11)
├── lightning_rod.png          (P12)
├── death_relic.png            (P13)
├── fire_rune.png              (P14)
├── magnet.png                 (P15)
└── clock.png                  (P16)
```

### Characters
```
characters/
├── raven.png                  (C01)
├── helga.png                  (C02)
├── spark.png                  (C03)
├── morgana.png                (C04)
├── thorn.png                  (C05)
├── zephyr.png                 (C06)
├── krion.png                  (C07)
├── volt.png                   (C08)
├── knox.png                   (C09)
├── pyros.png                  (C10)
├── archon.png                 (C11 premium)
├── nihil.png                  (C12 premium)
└── valkyrie.png               (C13 premium)
```

### Biomes (tile-наборы)
```
biomes/dark_forest/
├── tile_grass.png
├── tile_path.png
├── deco_tree.png              (коллизия)
├── deco_bush.png              (без коллизии)
├── deco_mushroom.png
├── deco_stump.png
└── deco_swamp.png             (замедление)

biomes/ice_wastes/
├── tile_snow.png
├── tile_ice.png               (скольжение)
├── deco_icicle.png
├── deco_snowdrift.png
└── deco_ice_crystal.png       (даёт руну Льда)

biomes/volcanic/
├── tile_stone.png
├── tile_lava.png              (урон)
├── deco_vent.png              (спавнит врагов)
├── deco_obsidian.png
└── deco_geyser.png

biomes/storm_citadel/
├── tile_metal.png
├── deco_lightning_rod.png     (притягивает молнии)
├── deco_crystal.png
└── deco_machine.png
```

## Fallback-система

Отсутствующие спрайты отрисовываются процедурно (см. `src/rendering/PlaceholderSprites.js`):
- Цветной круг/эллипс с обводкой и инициалом
- Цвет соответствует категории (стихия руны, тип врага и т.д.)
