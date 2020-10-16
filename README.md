# MSFS-Mod-Repository
An open source, license free repository of MSFS mod meta-information. Used by [MSFS Mod Selector](https://github.com/captn-nick/MSFS-Mod-Selector) for automatic mods lookup.

Current Status: **CLOSED** for contributions.

Contributions will be welcome once MSFS Mod Selector hits v. 0.8.

### Restrictions for contributions
In addition to the [restrictions for registering mods in your local repository](https://github.com/captn-nick/MSFS-Mod-Selector#restrictions), the following rules are enforced for mod registrations for the online mod DB repository:
* Mod type must not be “Other”.
* For all non-aircraft mod types, continent must be one of the supported continents except “Other/Fictional”.
* For all non-aircraft mod types, country must be one of the supported countries and must match the continent it is supposed to be linked to.
* For airport mods, ICAO must not be empty; if it is actually unknown / not set / multiple, must be explicitly denoted with a - (minus sign).
* For all aircraft mod types, continent must be one of the supported continents except “Other/Fictional”, or empty.
* For all aircraft mod types, country must be one of the supported countries and must match the continent it is supposed to be linked to; or it must be empty.
* For all aircraft mod types, aircraft type must be one of the supported aircraft types.
* For all mod types, description, author, and url must not be empty, and url must start with either "https://www.flightsim.to/file/” or "https://flightsim.to/file/”. The “www” url is preferred.

Please use the “Contribute to Mods DB” functionality to export your local mod definitions to the mods-db.txt repository. In this case, these rules will be enforced automatically.
Additionally, all mods will be automatically sorted alphabetically my mod name. This is important to minimize the risk and complexity of Git merge conflicts (compared to always adding new mod definitions simply at the end of the file).

Additionally, please respect the following rules:
* Please only assign a particular city to the mod in question if the mod is located within the actual city limits and if the city is of at least some national significance regarding its size. A good rule of thumb for the latter would be to not explicitly assign a particular city if its population is less than 100’000. This latter rule is in place so that the UI won’t be cluttered by hundreds of miniscule municipals.
* Cities shall take their local names (including all diacritics like ä, è, and ø), not the English translation, if they are written in the Latin alphabet; otherwise, the English translation shall be taken. For both cases, Wikipedia shall serve as the canonical source. For instance, write München instead of Munich and Roma instead of Rome, but Athens instead of Αθήνα or Athína and Tokyo instead of 東京 or Tōkyō.
