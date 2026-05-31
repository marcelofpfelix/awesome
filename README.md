# Awesome RTC

A curated list of open-source RTC, SIP, VoIP, WebRTC, RTP, STUN/TURN, and
media-observability software.

The scope is practical software for building, testing, operating, debugging, or
learning real-time communications systems. The list intentionally favors
projects with source-available implementations, reusable protocols, diagnostic
value, or established operational use.

## Selection Notes

- Open-source RTC/VoIP related projects only.
- Includes libraries, user agents, softphones, servers, media relays, gateways,
  diagnostic tools, scenario/load tools, and observability stacks.
- Excludes proprietary services, closed-source hosted products, and general
  networking tools unless they are commonly used for RTC/VoIP troubleshooting.
- Project fit depends on the use case: embedded libraries are useful for custom
  products, while subprocesses, containers, and full services are often better
  for labs, fixtures, and integration tests.

## SIP And VoIP User Agents

- PJSIP / `pjsua`: mature open-source SIP/media stack with a C API, CLI tools,
  NAT traversal support, and broad VoIP coverage.
- liblinphone / linphone-sdk: full-featured open-source SIP/VoIP SDK and client
  stack.
- `linphonec`: liblinphone console client, useful as a command/control and
  callback reference for call state, auth, DTMF, text, auto-answer, and
  daemon-style command handling.
- baresip: lightweight open-source SIP softphone stack and automation
  reference.
- MicroSIP: open-source Windows SIP softphone based on PJSIP.
- CSipSimple: open-source Android SIP softphone history and SIP/NAT behavior
  reference.
- Jitsi Desktop: open-source desktop SIP/XMPP softphone reference.
- Twinkle: open-source Linux SIP softphone reference.
- diago / sipgo: open-source Go references for SIP dialogs, RTP, DTMF, WAV, and
  media helpers.

## SIP Servers, PBX, Proxies, And B2BUA

- Kamailio: open-source SIP proxy/SBC/lab service and module-architecture
  reference.
- OpenSIPS: open-source SIP proxy/server and carrier-routing reference.
- Asterisk: open-source PBX and telephony application framework.
- FreeSWITCH: open-source PBX/media service for complex call-control and media
  scenarios.
- Flexisip: open-source SIP proxy, presence, and group-chat suite from
  Belledonne.
- drachtio: open-source SIP server framework for Node.js applications.
- reSIProcate / Repro: open-source SIP stack and federated SIP server.
- Routr: open-source lightweight SIP proxy, location server, and registrar.
- Sippy B2BUA: open-source Python back-to-back user-agent server.
- Sippy Go B2BUA: open-source Go back-to-back user-agent server.
- SEMS: open-source SIP media and application server.
- Siproxd: open-source SIP proxy/masquerading daemon.
- Dubango WebRTC2SIP: open-source SIP/WebRTC gateway reference.
- Kazoo: open-source carrier VoIP API platform built around FreeSWITCH and
  Kamailio.
- Wazo: open-source VoIP API platform built around Asterisk, Kamailio, and
  RTPEngine.
- FusionPBX: open-source FreeSWITCH web management and multitenant PBX system.
- FreePBX: open-source Asterisk web management system.
- Fonoster: open-source programmable telecom stack.
- jambonz: open-source CPaaS for SIP and programmable voice.
- IVOZ Provider: open-source multitenant VoIP provider platform.
- CGRateS: open-source carrier-grade rating and charging server.

## SIP Scenario And Load Tools

- SIPp: canonical open-source SIP scenario and load-generation tool with XML
  scenarios, CSV injection, rate controls, and trace/stat artifacts.
- Gossipper: open-source SIPp-compatible Go platform with RTP, HEP, reporting,
  and PCAP-to-scenario ideas.
- sipexer: open-source focused SIP CLI for OPTIONS, REGISTER, MESSAGE, INVITE,
  authentication, and transports.
- sipsak: open-source legacy SIP diagnostics.
- SIPVicious: open-source SIP security audit suite.
- SIPPTS: open-source SIP penetration-testing and protocol test toolkit.
- PROTOS SIP test suite: open-source malformed-SIP corpus for parser and
  robustness fixtures.
- sipcmd / sipcmd2: open-source command-line SIP call tools.
- telefonist: open-source SIP automation reference.
- wsctl: open-source WebSocket command-line tool from the Kamailio ecosystem.
- protos-sip / protoshoot: open-source SIP protocol test and raw-message
  shooting idea sources.

## SIP, RTP, And WebRTC Libraries

- PJSIP / PJPROJECT: open-source C SIP, media, and NAT traversal stack.
- liblinphone / linphone-sdk: open-source SIP/VoIP SDK and full client stack.
- libre / librem / baresip stack: open-source SIP, SDP, RTP/RTCP, STUN, TURN,
  ICE, and user-agent building blocks.
- oSIP / eXosip: open-source C SIP libraries for parser/dialog/user-agent
  primitives.
- Sofia-SIP: open-source C SIP library used by FreeSWITCH.
- reSIProcate: open-source C++ SIP stack.
- JAIN-SIP: open-source Java SIP stack.
- sipsorcery: open-source .NET SIP, SDP, RTP, STUN, and WebRTC stack.
- JsSIP: open-source JavaScript SIP-over-WebSocket library.
- SIP.js: open-source JavaScript SIP signaling library.
- sipML5 / sipML5-NG: open-source browser SIP/WebRTC client references.
- dart-sip-ua: open-source Dart port of JsSIP.
- RTCKit/PHP SIP: open-source PHP SIP parser and renderer.
- rsip: open-source Rust SIP parser/model reference.
- sipcore / libsip / parsip: open-source Rust SIP implementation ideas.
- pyVoIP: open-source Python VoIP library.
- ersip / NkSIP: open-source Erlang SIP building blocks.
- Pion WebRTC: open-source Go WebRTC stack.
- Pion TURN: open-source Go TURN toolkit.
- aiortc: open-source Python WebRTC behavior reference.
- libdatachannel: open-source C++ WebRTC data-channel and media-transport
  library.
- datachannel-wasm: open-source WebAssembly build of libdatachannel.
- rawrtc: open-source WebRTC/ORTC C library.
- werift: open-source TypeScript WebRTC implementation.
- node-datachannel: open-source Node bindings for libdatachannel.
- node-webrtc: open-source Node bindings for WebRTC.
- rtcrs/webrtc: open-source Rust WebRTC stack.

## Network, Media, NAT, And Observability

- STUNTMAN: open-source STUN/NAT behavior checks through `stunclient` and a
  fixture server.
- coturn: open-source TURN/STUN server and common VoIP/WebRTC lab dependency
  for TURN allocation, relay, auth, TLS, and DTLS validation.
- eturnal: open-source Erlang STUN/TURN server.
- turn-rs: open-source Rust TURN server.
- violet: open-source lightweight STUN/TURN server.
- natcheck: open-source NAT behavior diagnosis CLI.
- STUNner: open-source Kubernetes media gateway for WebRTC.
- rtpengine: open-source RTP/media relay validation and SBC media-path parity.
- RTPProxy: open-source RTP relay and NAT/media-path reference.
- erlrtpproxy / pylrkproxy: open-source RTP proxy variants.
- HEP / HOMER ecosystem: open-source passive SIP/RTC capture interoperability
  and ladder/reporting model.
- sngrep: open-source SIP ladder troubleshooting reference.
- sipgrep: open-source SIP packet sniffing and console exploration tool.
- SIP3: open-source VoIP/RTC traffic monitoring and analysis platform.
- rtpbreak / rtpsplit: open-source RTP reconstruction and analysis reference.
- WebRTC Troubleshooter: open-source client-side WebRTC diagnostics reference.
- Trickle ICE sample: open-source client-side ICE/NAT debug reference.
- tcpdump / tshark / Wireshark: open-source packet capture and decode
  references often used in RTC/VoIP investigations.

## WebRTC Servers, Gateways, And Media Apps

- Janus Gateway: open-source WebRTC gateway and media server.
- LiveKit: open-source WebRTC SFU/media infrastructure.
- mediasoup: open-source WebRTC SFU and conferencing framework.
- Jitsi Videobridge / Jitsi Meet: open-source WebRTC conferencing and SFU
  reference stack.
- Kurento: open-source WebRTC media server with media processing and recording.
- Galene: open-source lightweight video-conference server.
- OpenVidu: open-source video-conference platform built on WebRTC.
- BigBlueButton: open-source web conferencing system.
- MiroTalk P2P / SFU: open-source WebRTC meeting references.
- Plug-N-Meet: open-source conferencing system built around LiveKit.
- Medooze Media Server: open-source Node WebRTC media server.
- Kraken: open-source Go WebRTC SFU.
- OvenMediaEngine / OvenPlayer: open-source low-latency media streaming
  reference.
- selkies-gstreamer: open-source low-latency Linux WebRTC and GStreamer remote
  desktop/media components.
- Pipecat: open-source voice/media pipeline reference.
- VoiceBlender: open-source SIP/WebRTC/AI voice service idea source.
- Gossipper WebRTC: open-source experimental WebRTC bridge ideas.

## Practical Notes

- Choose embedded libraries when you need tight control over protocol behavior
  or application integration.
- Choose existing CLI tools and services for repeatable labs, black-box
  interoperability checks, and operational diagnostics.
- Choose full media servers, relays, and gateways when the test needs real
  media-path behavior, NAT traversal, recording, conferencing, or SFU/MCU
  semantics.
