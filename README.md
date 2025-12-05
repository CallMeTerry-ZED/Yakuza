[![Build status](https://github.com/networkprotocol/yojimbo/workflows/CI/badge.svg)](https://github.com/networkprotocol/yakuza/actions?query=workflow%3ACI)

# yakuza

**yakuza** is a network library for client/server games written in C++.

It's designed around the networking requirements of competitive multiplayer games like first person shooters. 

Generally speaking, if you have a custom game engine written in C++ and you want to network your game, yakuza is a really good choice.

![image](https://github.com/mas-bandwidth/yojimbo/assets/696656/098935f2-ba2b-4540-8d7f-474acc7f2cd8)

It has the following features:

* Cryptographically secure authentication via [connect tokens](https://github.com/networkprotocol/netcode/blob/master/STANDARD.md)
* Client/server connection management and timeouts
* Encrypted and signed packets sent over UDP
* Packet fragmentation and reassembly
* Bitpacker and serialization system
* Unreliable-unordered messages for time sensitive data
* Reliable-ordered messages with aggressive resend until ack
* Data blocks larger than maximum packet size can be attached to reliable-ordered messages
* Estimates of latency, jitter, packet loss, bandwidth sent, received and acked per-connection

yakuza is stable and production ready.

## Source Code

You can get the latest source code by cloning it from github:

      git clone https://github.com/mas-bandwidth/yakuza.git
      
## Author

The Original author of this library(yojimbo) is [Glenn Fiedler](https://www.linkedin.com/in/glenn-fiedler-11b735302/).
I have editied it to be my own Networking Libaray.

yakuza is built on top of other open source libraries by the same author: [netcode](https://github.com/mas-bandwidth/netcode), [reliable](https://github.com/mas-bandwidth/reliable), and [serialize](https://github.com/mas-bandwidth/serialize)

## License

[BSD 3-Clause license](https://opensource.org/licenses/BSD-3-Clause).
