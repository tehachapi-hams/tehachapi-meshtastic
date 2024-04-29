# Portals

## MQTT Portals

Setting up a "public" MQTT server is actually a lot of effort, and a chore I'm
not super interested in. If we reach a size of where it would become useful to
have one, that works for nodes with internet connections, I will consider it.

### `downtown-01` <--> `alpine-village-01`

Both of these nodes are bridged via a private MQTT server, meaning anything
that hits Alpine, will be re-broadcast in Downtown Tehachapi and vice versa.
