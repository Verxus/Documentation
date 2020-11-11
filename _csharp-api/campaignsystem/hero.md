# Hero : [MBObjectBase](), [ITrackableCampaignObject](), [ITrackableBase]()

Heroes are all the unique characters in the game. This class contains all the information of these characters and allows you to change them.

| Using / Namespaces                                                              | <div style='color:yellow'>Taleworlds.Core</div> | <div style='color:green'>Saveable</div> |
| :------------------------------------------------------------------------------ | ----------------------------------------------- | --------------------------------------: |
| `System`                                                                        |                                                 |                                   20204 |
| `System.Collections.Generic`                                                    |                                                 |                                         |
| `System.Linq`                                                                   |                                                 |                                         |
| `System.Xml.Serialization`                                                      |                                                 |                                         |
| `Helpers`                                                                       |                                                 |                                         |
| [TaleWorlds.CampaignSystem.Actions](./actions/ChangeOwnerOfSettlementAction.md) |                                                 |                                         |
| [TaleWorlds.CampaignSystem.CharacterDevelopment.Managers]()                     |                                                 |                                         |
| [TaleWorlds.Core](../core/README.md)                                            |                                                 |                                         |
| [TaleWorlds.Library](../library/README.md)                                      |                                                 |                                         |
| [TaleWorlds.Localization](../localization/README.md)                            |                                                 |                                         |
| [TaleWorlds.SaveSystem](../savesystem/README.md)                                |                                                 |                                         |
|                                                                                 |

## Example of usage

TODO

## Variables

 | Mods              | Name                          | Type                                                           | Notes                                      | Value |
 | ----------------- | ----------------------------- | -------------------------------------------------------------- | ------------------------------------------ | ----- |
 | public const      | RelationLimit                 | `int`                                                          | Max value for relation                     | 100   |
 | public const      | RelationNeutralLimit          | `int`                                                          | Max value for relation with neutral heroes | 10    |
 | public            | LastTimeStampForActivity      | `int`                                                          | Last activity timestamp                    |       |
 | const             | MaximumNumberOfVolunteers     | `int`                                                          | TODO                                       | 6     |
 | public            | VolunteerTypes;               | [CharacterObject]()`[]`                                        | TODO                                       |       |
 | public            | NumberOfCreatedParties        | `int`                                                          | Number of parties                          |       |
 | private readonly  | _occupiedByAnEvent            | `List<string>`                                                 | TODO                                       |       |
 | private           | _passedTimeAtHomeSettlement;  | `float`                                                        | Time at home settlement                    |       |
 | private           | _characterObject              | [CharacterObject]()                                            | Character object info                      |       |
 | public            | FirstName                     | [TextObject]()                                                 | First name                                 |       |
 | public            | Name                          | [TextObject]()                                                 | Name                                       |       |
 | public            | Detected                      | `bool`                                                         | Have you met with hero                     |       |
 | public            | DaysLeftToRespawn             | `int`                                                          | Days for respawn                           |       |
 | private           | _heroStates                   | [CharacterStates](##-`enum`-CharacterStates)                   | Hero's state                               |       |
 | private           | _heroTraits                   | [CharacterTraits]()                                            | Hero's traits                              |       |
 | private           | _heroPerks                    | [CharacterPerks]()                                             | Hero's perks                               |       |
 | private           | _heroSkills                   | [CharacterSkills]()                                            | Hero's skills                              |       |
 | private           | _charAttributeValues          | `int[6]`                                                       | Character attributes points                |       |
 | public            | NeverBecomePrisoner           | `bool`                                                         | Will never be prisoner?                    |       |
 | private           | _alwaysUnconscious;           | `bool`                                                         | TODO                                       |       |
 | public            | AlwaysDie                     | `bool`                                                         | Is hero always dir (for what?)             |       |
 | public            | LastVisitTimeOfHomeSettlement | `float`                                                        | Last visit home settlement                 |       |
 | public            | Level                         | `int`                                                          | Level of hero                              |       |
 | const             | HeroWoundedHealthLevel        | `int`                                                          | Value, below which hero is wounded         | 20    |
 | private           | _companionOf                  | [Clan]()                                                       | Clan that include hero?                    |       |
 | private           | _cachedLastSeenInformation    | [HeroLastSeenInformation](##-`struct`-HeroLastSeenInformation) | Heros's last seen info                     |       |
 | IsMercenary       | IsMercenary                   | `bool`                                                         | Is hero mercenary                          |       |
 | SpcDaysInLocation | SpcDaysInLocation             | `int`                                                          | TODO                                       |       |
 | private           | _health                       | `int`                                                          | Health                                     |       |
 | private           | _birthDay                     | [CampaignTime]()                                               | BirthDay                                   |       |
 | private           | _deathDay                     | [CampaignTime]()                                               | Day of death                               |       |
 | private           | _power                        | `int`                                                          | Power                                      |       |
 | public            | VisitedSettlements            | `Dictionary<`[Settlement]()`, float>`                          | Visited settlements                        |       |
 | private           | _clan                         | [Clan]()                                                       | Hero's clan                                |       |
 | private           | _supporterOf                  | [Clan]()                                                       | TODO                                       |       |
 | private           | _governorOf                   | [Town]()                                                       | Governor of                                |       |
 | private           | _ownedWorkshops               | `List<`[Workshop]()`>`                                         | Owned workshops                            |       |
 | private           | _ownedCommonAreas             | `List<`[CommonArea]()`>`                                       | Owned areas                                |       |
 | private           | _ownedParties                 | `List<`[PartyBase]()`>`                                        | Owned parties                              |       |
 | public            | Culture                       | [CultureObject]()                                              | Culture                                    |       |
 | public            | _partyBelongedTo              | [MobileParty]()                                                | TODO                                       |       |
 | private           | _stayingInSettlementOfNotable | [Settlement]()                                                 | TODO                                       |       |
 | public            | SpecialItems                  | `List<`(ItemObject)[]`>`                                       | TODO                                       |       |
 | private           | _controversy                  | `float`                                                        | TODO                                       |       |
 | private           | _hasMet                       | `bool`                                                         | Has hero met                               |       |
 | private           | _bornSettlement               | [Settlement]()                                                 | Born settlement                            |       |
 | private           | _gold                         | `int`                                                          | Gold                                       |       |
 | public            | RandomValue                   | `int`                                                          | ??                                         |       |
 | public            | RandomValueDeterministic      | `int`                                                          | ??                                         |       |
 | public            | RandomValueRarelyChanging     | `int`                                                          | ??                                         |       |
 | private           | _father                       | [Hero]()                                                       | Father                                     |       |
 | private           | _mother                       | [Hero]()                                                       | Mother                                     |       |
 | private readonly  | _exSpouses                    | `List<`[Hero]()`>`                                             | ??                                         |       |
 | public            | ExSpouses                     | [MBReadOnlyList]()`<`[Hero]()`>`                               | Ex. spouses                                |       |
 | private           | _spouse                       | [Hero]()                                                       | Spouse                                     |       |
 | private readonly  | _children                     | `List`[Hero]()`>`                                              | Children                                   |       |
 | public            | IsFertile                     | bool                                                           | Can hero have children                     |       |
 | public            | IsPregnant                    | bool                                                           | Is hero pregnant now                       |       |
 | private readonly  | _heroDeveloper                | [HeroDeveloper]()                                              | TODO                                       |       |
 |                   |


## Properties

- `internal StaticBodyProperties StaticBodyProperties` { get; set; }
- `CanHaveRecruits` - A boolean that details if this hero can have recruits. Preachers, Rural Notables, Mercenaries, Gang Leaders, Merchants, and Headmen can have recruits. This property can only be read, not changed.

## Functions

Work in progress


## `struct` HeroLastSeenInformation

 | Name               | Type             | Notes |
 | ------------------ | ---------------- | ----- |
 | LastSeenPlace      | [Settlement]()   | TODO  |
 | LastSeenDate       | [CampaignTime]() | TODO  |
 | IsNearbySettlement | bool             | TODO  |
 |                    |

## `enum` CharacterStates

* NotSpawned
* Active
* Fugitive
* Prisoner
* Released
* Dead
* Disabled

## `enum` FactionRank

* None = -1
* Vassal
* Leader
