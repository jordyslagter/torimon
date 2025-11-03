# Software Requirements Specification

This document details the functional and non-functional requirements for the
artefact.

## Owners

| Name      | Description                                                                                      |
| --------- | ------------------------------------------------------------------------------------------------ |
| User      | A normal player that plays the modpack locally or via a server                                   |
| Moderator | A user with elevated permissions that oversees other users and prevents and resolves rule breaks |

## Functional requirements

| ID   | Requirement                                                             | Owner     | Priority    |
| ---- | ----------------------------------------------------------------------- | --------- | ----------- |
| FR01 | The user accesses Pokémon                                               | User      | Must have   |
| FR02 | The user mega-evolves a Pokémon                                         | User      | Should have |
| FR03 | The user accesses a minimap                                             | User      | Must have   |
| FR04 | The user plays with other users via a server                            | User      | Must have   |
| FR05 | The user plays with other users over the internet via their own machine | User      | Could have  |
| FR06 | The user accesses a web-based map for a server                          | User      | Could have  |
| FR07 | The user can not encounter hostile mobs                                 | User      | Must have   |
| FR08 | The user plays with the hunger system active                            | User      | Must have   |
| FR09 | The user signs up to the game server via the Discord server             | User      | Should have |
| FR10 | The moderator views responsibility for placed/destroyed blocks          | Moderator | Must have   |
| FR11 | The user accesses seasons                                               | User      | Should have |

## Non-functional requirements

| ID   | Requirement                                                          | System  | Priority    |
| ---- | -------------------------------------------------------------------- | ------- | ----------- |
| NF01 | The server can update the modpack automatically                      | Server  | Must have   |
| NF02 | The interval at which the server updates the modpack is configurable | Server  | Must have   |
| NF03 | The modpack only contains mods from Modrinth                         | Modpack | Should have |
| NF04 | The modpack disables chat reporting to official Mojang servers       | Modpack | Must have   |
| NF05 | The modpack does not contain telemetry collection                    | Modpack | Must have   |
| NF06 | The modpack does not contain sponsor-only content                    | Modpack | Should have |
| NF07 | The modpack does not contain recipe conflicts                        | Modpack | Should have |
| NF08 | The modpack compiles in-game guides into one                         | Modpack | Could have  |
