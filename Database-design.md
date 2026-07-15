# Pokemon GO Hub Database Design

## Pokemon

| Field | Type | Description |
|-------|------|-------------|
| id | integer | Internal ID |
| name | text | Pokemon name |
| pokedex_number | integer | National dex number |
| type1 | text | Primary type |
| type2 | text | Secondary type |
| attack | integer | Pokemon GO attack stat |
| defense | integer | Pokemon GO defense stat |
| stamina | integer | Pokemon GO stamina stat |
| is_shadow_available | boolean | Has a shadow form |
| is_mega_available | boolean | Has a mega evolution |
| is_gmax_available | boolean | has a Gmax form |
| image_url | text | Pokemon image |

---

## Moves

| Field | Type | Description |
|-------|------|-------------|
| id | integer | Move ID |
| name | text | Move name |
| move_type | text | Fire, Water, Dragon, etc |
| category | text | Fast or Charged |
| power | integer | Damage |
| energy | integer | Energy generation or cost |

---

## Counters

| Field | Type | Description |
|-------|------|-------------|
| target_pokemon_id | integer | Pokemon being countered |
| counter_pokemon_id | integer | Counter Pokemon |
| score | decimal | Counter effectiveness score |

---

## Rankings

| Field | Type | Description |
|-------|------|-------------|
| id | integer | Internal ID |
| category | text | Fast or Charged |
| type1 | text | Primary type |
| type2 | text | Secondary type |
| rank | integer | position in rankings |

---

## Types

| Field | Type | Description |
|-------|------|-------------|
| type_name | text | pokemon type name |
| strong_against | array | typings pokemon is effect or super effective against |
| weak_against | array | typings pokemon is weak to |
| resists | array | types it resists |

---



#############################################################
## For Future
## Rarity
| Field | type | Description |
|-------|------|-------------|
| id | integer | Internal ID |
| name | text | Pokemon name |
| pokedex_number | integer | national dex number |
| cp | integer | battle power |
| iv_attack | integer | attack value |
| iv_defense | integer | defense value |
| iv_hp | integer | hp value | 
| lucky | boolean | whether it is lucky or not |
| shiny | boolean | whether it is shiny or not |
| costume | boolean | whether it is costume or not |
| background | boolean | whether it has background or not |
| shadow | boolean | whether it is shadow or not |
| gmax_form | boolean | whether it has a Gmax form or not |
| mega_evolution | boolean | whether it has Mega Evolution  or not |
