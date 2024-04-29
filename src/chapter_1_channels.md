# Channels

The current channel layout, for the Tehachapi Meshtastic network, is laid out like so.

## Configuration Reference

- [Meshtastic Channel Documentation](https://meshtastic.org/docs/configuration/radio/channels/)

## Tehachapi Meshtastic Channels (Required)

Nodes in the network, MUST operate with these general settings.

| Index | Channel | Default Role  |  Name        | Purpose                                    | Encryption Setting  | Last Change |
| :---: | :-----: | :-----------: | :----------: | :----------------------------------------: | :-----------------: | :---------: |
|   0   |    1    |  `PRIMARY`    | `tm-pri`     | (telemetry) Open Network Channel           | `none`              | 2024-04-29  |
|   1   |    2    |  `SECONDARY`  | `tm-gen`     | (chat) Open General Chat Channel           | `none`              | 2024-04-29  |
|   2   |    3    |  User Defined | User defined | User Defined                               |                     |             |
|   3   |    4    |  User Defined | User defined | User Defined                               |                     |             |
|   4   |    5    |  User Defined | User defined | User Defined                               |                     |             |
|   5   |    6    |  User Defined | User defined | User Defined                               |                     |             |
|   6   |    7    |  User Defined | User defined | User Defined                               |                     |             |
|   7   |    8    |  `SECONDARY`  | RESERVED     | RESERVED (likely for an admin channel)     |                     | 2024-04-29  |

General things to know:

- The encryption setting of `none` is set to meet opinions of ham radio
  operators, because it allows the most number of Ham's to help the network
  with stronger transmissions that unlicensed users cannot perform.
  - Since we would intend to publish an encryption key here anyways, encrypted
    traffic is an allowed mode of operation since the key is published. But
    some folks don't get it.
- There is not yet a shared `admin` channel. That may change at some point in
  the future, but for now, you must run your own. (This is why Channel 8 is
  **RESERVED**)
- There can be no gaps between channels. You can't have Channel 8, if you don't
  also have Channels 1-7 setup.

## Carried Tehachapi Meshtastic Channels (Optional)

Nodes in the network, MAY carry optional channels, that are not defined in the
MUST category. It is recommended, that they do use encryption, to avoid message
stream overlap when channel overlap is necessary.

Encrypted channels, may or may not have a published static encryption key. If
the key is not published here, it is unlikely that it would be syndicated by
more powerful Ham Operator nodes.

| Index | Channel | Default Role  |  Name        | Purpose                                    | Encryption Setting  | Last Change |
| :---: | :-----: | :-----------: | :----------: | :----------------------------------------: | :-----------------: | :---------: |
