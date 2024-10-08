# Channels

The current channel layout, for the Tehachapi Meshtastic network, is laid out like so.

## QR Code

A shortcut, to getting everything dialed in, is available by using the Meshtastic App with this QR Code.

![Map, as of May 2nd, 2024](./images/tehachapi-meshtastic-qrcode-20240821.png)

## Configuration Reference

- [Meshtastic Channel Documentation](https://meshtastic.org/docs/configuration/radio/channels/)

## Tehachapi Meshtastic Channels (Strongly Suggested To Start)

Nodes in the network, with the exception of Default Role, SHOULD operate with these general settings:

| Index | Channel | Default Role  |  Name        | Purpose                                    | Encryption Setting        | Last Change |
| :---: | :-----: | :-----------: | :----------: | :----------------------------------------: | :-----------------------: | :---------: |
|   0   |    1    |  `PRIMARY`    | `tm-pri`     | (telemetry) Open Network Channel           | `default` (aka `0x01`)    | 2024-08-21  |
|   1   |    2    |  `SECONDARY`  | `tm-gen`     | (chat) Open General Chat Channel           | `default` (aka `0x01`)    | 2024-08-21  |
|   2   |    3    |  User Defined | User defined | User Defined                               |                           |             |
|   3   |    4    |  User Defined | User defined | User Defined                               |                           |             |
|   4   |    5    |  User Defined | User defined | User Defined                               |                           |             |
|   5   |    6    |  User Defined | User defined | User Defined                               |                           |             |
|   6   |    7    |  User Defined | User defined | User Defined                               |                           |             |
|   7   |    8    |  User Defined | User defined | User Defined                               |                           | 2024-08-07  |

Variances:

- You are not required to use these same settings, especially for a PRIMARY channel.
  - It is recommended to try them like this to start, with low accuracy on your postion.
  - You can privately share your position, and change your PRIMARY channel (see [details here](https://meshtastic.org/docs/configuration/tips/#not-sharing-your-location)).
- If you remain in `LONG_FAST`, your messages in general will still be routed by the network,
  regardless of if you share the same tooling or not. 

General things to know:

- Currently, the `tm-pri` channel often has automatic "reply" messages being
  sent from it, just for folks to test connectivity quickly.
  - Traceroute is another useful tool for this.
  - At this point in time, Range Test should feel free to operate in here.
- The encryption setting of `default` (the trivial key of "1") is now set to
  match the convenience of new users on the network.
  - Ham Radio operators should note that this is a **PUBLISHED KEY** on this
    **PUBLIC WEBPAGE**, and the intent is not to `obscure meaning`.
  - At this time, we have recieved no contact from an FCC Regional Director
    under §97.309(b) restricting our usage.
  - All records, if they were required to be kept, are already recorded in
    this `git` repository.
- There can be no gaps between channels. You can't have Channel 8, if you don't
  also have Channels 1-7 setup.

## Carried Tehachapi Meshtastic Channels (Optional)

Nodes in the network, MAY carry optional channels, or sister mesh channels.

Encrypted channels, may or may not have a published static encryption key. If
the key is not published here, it is unlikely that it would be syndicated by
more powerful Ham Operator nodes.

| Index | Channel | Default Role  |  Name        | Purpose                                    | Encryption Setting  | Last Change |
| :---: | :-----: | :-----------: | :----------: | :----------------------------------------: | :-----------------: | :---------: |
