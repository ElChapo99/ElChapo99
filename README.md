tasks:
  harvest:
    type: "mobkilling"
    mob: BLAZE
    amount: 200
display:
  name: "&aCazador de Blaze &e#1"
  lore-normal:
    - "&8Misiones de progreso."
    - ""
    - "&7Tienes que matar 200 BLAZE"
    - "&7Progreso: &6{harvest:progress}/200 BLAZE."
    - ""
    - "&fRecompensas:"
    - "&7- &a&l$&a50,000&f."
  lore-started:
    - "&r"
    - "&fEstado: &a&lINICIADA"
# Here you can list messages which will be sent to the player (if they are online) upon the quest starting.
startstring:
  - "&7&m-----------------------------------"
  - "&7"
  - "&f¡Tienes una nueva &a&lMISIÓN!"
  - "&fObjetivo: &eMatar 200 BLAZE"
  - "&7"
  - "&7Al completar esta misión"
  - "&7serás recompensado con &a&l$&a50,000"
  - "&7"
  - "&7&m-----------------------------------"
rewards:
  - "eco give {player} 50000"
# Here you can list messages which will be sent to the player (if they are online) upon completion.
rewardstring:
  - " &8■ &a&l$&a50,000 &7se agregó a tu saldo en el juego."

# These placeholders are accessible using PlaceholderAPI, for example %quests_tracked_p:description%
# They are useful for putting information about the players tracked quest on a scoreboard
# You may want to keep the names of them the same for ALL quests for this use-case
placeholders:
  description: "&9Mata 200 BLAZE."
  progress: " &8- &9{harvest:progress}/200"  
  
options:
  category: "blaze"
  requires: []
  repeatable: false
  cooldown:
    enabled: false
    time: 82600
  sort-order: 1
