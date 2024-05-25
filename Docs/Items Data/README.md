# Items Data

This is special file, which is used for getting items names, texture files and coordinates, behavior and other stuff. It is also useful to know as it is used in multiple packets.

It is possible to first decoded items database on [this page](https://wombat.platymuus.com/growtopia/itemdb.php). Also based on this page was first [items dat decoder](https://github.com/GrowtopiaNoobs/Growtopia_ItemsDecoder) created.

> [!TIP]
> Use latest Items Data Encoder & Decoder like [GrowTools](https://github.com/GuckTubeYT/GrowtTools), and [GoDat](https://github.com/Eikarna/GoDat).

## Items data structure

This structure begins with information about file and then this is followed by adding all items one after another.

Beginning structure:

uint16 for file version - this is updated when new fields are added
uint32 for item count

This is followed by all those items, items structure are following:

- uint32 - item ID, starting from zero
- uint8 - ...
- uint8 - ...
- uint8 - ...
- uint8 - ...
- string - item name, it is [encoded using simple cipher](cipher.md)
- ... TODO
