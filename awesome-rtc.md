# Awesome RTC

A curated list of open-source SIP, RTP, WebRTC, STUN/TURN, and IMS software.
media-observability software.

## SIP And VoIP User Agents

- [PJSIP / `pjsua`](https://github.com/pjsip/pjproject): mature open-source
  SIP/media stack with a C API, CLI tools, NAT traversal support, and broad
  VoIP coverage.
- [liblinphone / linphone-sdk](https://gitlab.linphone.org/BC/public/linphone-sdk):
  full-featured open-source SIP/VoIP SDK and client stack.
- [`linphonec`](https://gitlab.linphone.org/BC/public/linphone-sdk): liblinphone
  console client, useful as a command/control and callback reference for call
  state, auth, DTMF, text, auto-answer, and daemon-style command handling.
- [baresip](https://github.com/baresip/baresip): lightweight open-source SIP
  softphone stack and automation reference.
- [MicroSIP](https://github.com/MicroSIP/MicroSIP): open-source Windows SIP
  softphone based on PJSIP.
- [CSipSimple](https://github.com/r3gis3r/CSipSimple): open-source Android SIP
  softphone history and SIP/NAT behavior reference.
- [Jitsi Desktop](https://github.com/jitsi/jitsi): open-source desktop SIP/XMPP
  softphone reference.
- [Twinkle](https://github.com/LubosD/twinkle): open-source Linux SIP softphone
  reference.
- [diago](https://github.com/emiago/diago) /
  [sipgo](https://github.com/emiago/sipgo): open-source Go references for SIP
  dialogs, RTP, DTMF, WAV, and media helpers.

[Back to top](#awesome-rtc)

## SIP Servers, PBX, Proxies, And B2BUA

- [Kamailio](https://github.com/kamailio/kamailio): open-source SIP
  proxy/SBC/lab service and module-architecture reference.
- [OpenSIPS](https://github.com/OpenSIPS/opensips): open-source SIP
  proxy/server and carrier-routing reference.
- [Asterisk](https://github.com/asterisk/asterisk): open-source PBX and
  telephony application framework.
- [FreeSWITCH](https://github.com/signalwire/freeswitch): open-source PBX/media
  service for complex call-control and media scenarios.
- [Flexisip](https://gitlab.linphone.org/BC/public/flexisip): open-source SIP
  proxy, presence, and group-chat suite from Belledonne.
- [drachtio](https://github.com/drachtio/drachtio-server): open-source SIP
  server framework for Node.js applications.
- [reSIProcate / Repro](https://github.com/resiprocate/resiprocate): open-source
  SIP stack and federated SIP server.
- [Routr](https://github.com/fonoster/routr): open-source lightweight SIP proxy,
  location server, and registrar.
- [Sippy B2BUA](https://github.com/sippy/b2bua): open-source Python
  back-to-back user-agent server.
- [Sippy Go B2BUA](https://github.com/sippy/go-b2bua): open-source Go
  back-to-back user-agent server.
- [SEMS](https://github.com/sems-server/sems): open-source SIP media and
  application server.
- [Siproxd](https://sourceforge.net/projects/siproxd/): open-source SIP
  proxy/masquerading daemon.
- [Dubango WebRTC2SIP](https://github.com/DoubangoTelecom/webrtc2sip):
  open-source SIP/WebRTC gateway reference.
- [Kazoo](https://github.com/2600hz/kazoo): open-source carrier VoIP API
  platform built around FreeSWITCH and Kamailio.
- [Wazo](https://github.com/wazo-platform/wazo-platform): open-source VoIP API
  platform built around Asterisk, Kamailio, and RTPEngine.
- [FusionPBX](https://github.com/fusionpbx/fusionpbx): open-source FreeSWITCH
  web management and multitenant PBX system.
- [FreePBX](https://github.com/FreePBX/framework): open-source Asterisk web
  management system.
- [Fonoster](https://github.com/fonoster/fonoster): open-source programmable
  telecom stack.
- [jambonz](https://github.com/jambonz/jambonz-feature-server): open-source
  CPaaS for SIP and programmable voice.
- [IVOZ Provider](https://github.com/irontec/ivozprovider): open-source
  multitenant VoIP provider platform.
- [CGRateS](https://github.com/cgrates/cgrates): open-source carrier-grade
  rating and charging server.

[Back to top](#awesome-rtc)

## SIP Scenario And Load Tools

- [SIPp](https://github.com/SIPp/sipp): canonical open-source SIP scenario and
  load-generation tool with XML scenarios, CSV injection, rate controls, and
  trace/stat artifacts.
- [Gossipper](https://github.com/sipcapture/gossipper): open-source
  SIPp-compatible Go platform with RTP, HEP, reporting, and PCAP-to-scenario
  ideas.
- [sipexer](https://github.com/miconda/sipexer): open-source focused SIP CLI
  for OPTIONS, REGISTER, MESSAGE, INVITE, authentication, and transports.
- [sipsak](https://github.com/nils-ohlmeier/sipsak): open-source legacy SIP
  diagnostics.
- [SIPVicious](https://github.com/EnableSecurity/sipvicious): open-source SIP
  security audit suite.
- [SIPPTS](https://github.com/Pepelux/sippts): open-source SIP
  penetration-testing and protocol test toolkit.
- [sipcmd](https://github.com/tmakkonen/sipcmd) /
  [sipcmd2](https://github.com/guisousanunes/sipcmd2): open-source command-line
  SIP call tools.
- [telefonist](https://github.com/negbie/telefonist): open-source SIP
  automation reference.
- [wsctl](https://github.com/kamailio/kamailio/tree/master/misc/tools/wsctl):
  open-source WebSocket command-line tool from the Kamailio ecosystem.
- [protos-sip](https://gitlab.com/kalilinux/packages/protos-sip): open-source SIP
  protocol test source package.
- [protoshoot](https://github.com/kamailio/kamailio/tree/master/misc/tools/protoshoot):
  open-source raw-message shooting idea source from the Kamailio tree.

[Back to top](#awesome-rtc)

## SIP, RTP, And WebRTC Libraries

- [PJSIP / PJPROJECT](https://github.com/pjsip/pjproject): open-source C SIP,
  media, and NAT traversal stack.
- [liblinphone / linphone-sdk](https://gitlab.linphone.org/BC/public/linphone-sdk):
  open-source SIP/VoIP SDK and full client stack.
- [libre](https://github.com/baresip/re) /
  [librem](https://github.com/baresip/rem) /
  [baresip](https://github.com/baresip/baresip): open-source SIP, SDP,
  RTP/RTCP, STUN, TURN, ICE, and user-agent building blocks.
- [oSIP](https://git.savannah.gnu.org/cgit/osip.git) /
  [eXosip](https://git.savannah.nongnu.org/cgit/exosip.git): open-source C SIP
  libraries for parser/dialog/user-agent primitives.
- [Sofia-SIP](https://github.com/freeswitch/sofia-sip): open-source C SIP
  library used by FreeSWITCH.
- [reSIProcate](https://github.com/resiprocate/resiprocate): open-source C++
  SIP stack.
- [JAIN-SIP](https://github.com/usnistgov/jsip): open-source Java SIP stack.
- [sipsorcery](https://github.com/sipsorcery-org/sipsorcery): open-source .NET
  SIP, SDP, RTP, STUN, and WebRTC stack.
- [JsSIP](https://github.com/versatica/JsSIP): open-source JavaScript
  SIP-over-WebSocket library.
- [SIP.js](https://github.com/onsip/SIP.js): open-source JavaScript SIP
  signaling library.
- [sipML5](https://github.com/DoubangoTelecom/sipml5) /
  [sipML5-NG](https://github.com/cloudonix/sipml5-ng): open-source browser
  SIP/WebRTC client references.
- [dart-sip-ua](https://github.com/flutter-webrtc/dart-sip-ua): open-source
  Dart port of JsSIP.
- [RTCKit/PHP SIP](https://github.com/rtckit/php-sip): open-source PHP SIP
  parser and renderer.
- [rsip](https://github.com/Televiska/rsip): open-source Rust SIP parser/model
  reference.
- [sipcore](https://github.com/kurotych/sipcore): open-source Rust SIP
  implementation idea.
- [libsip](https://github.com/ByteHeathen/libsip): open-source Rust SIP
  implementation idea.
- [parsip](https://github.com/kamarkiewicz/parsip): open-source Rust SIP parser
  implementation idea.
- [pyVoIP](https://github.com/tayler6000/pyVoIP): open-source Python VoIP
  library.
- [ersip](https://github.com/poroh/ersip) /
  [NkSIP](https://github.com/NetComposer/nksip): open-source Erlang SIP
  building blocks.
- [Pion WebRTC](https://github.com/pion/webrtc): open-source Go WebRTC stack.
- [Pion TURN](https://github.com/pion/turn): open-source Go TURN toolkit.
- [aiortc](https://github.com/aiortc/aiortc): open-source Python WebRTC
  behavior reference.
- [libdatachannel](https://github.com/paullouisageneau/libdatachannel):
  open-source C++ WebRTC data-channel and media-transport library.
- [datachannel-wasm](https://github.com/paullouisageneau/datachannel-wasm):
  open-source WebAssembly build of libdatachannel.
- [rawrtc](https://github.com/rawrtc/rawrtc): open-source WebRTC/ORTC C
  library.
- [werift](https://github.com/shinyoshiaki/werift-webrtc): open-source
  TypeScript WebRTC implementation.
- [node-datachannel](https://github.com/murat-dogan/node-datachannel):
  open-source Node bindings for libdatachannel.
- [node-webrtc](https://github.com/node-webrtc/node-webrtc): open-source Node
  bindings for WebRTC.
- [rtcrs/webrtc](https://github.com/rtcrs/webrtc): open-source Rust WebRTC
  stack.

[Back to top](#awesome-rtc)

## Network, Media, NAT, And Observability

- [STUNTMAN](https://github.com/jselbie/stunserver): open-source STUN/NAT
  behavior checks through `stunclient` and a fixture server.
- [coturn](https://github.com/coturn/coturn): open-source TURN/STUN server and
  common VoIP/WebRTC lab dependency for TURN allocation, relay, auth, TLS, and
  DTLS validation.
- [eturnal](https://github.com/processone/eturnal): open-source Erlang
  STUN/TURN server.
- [turn-rs](https://github.com/mycrl/turn-rs): open-source Rust TURN server.
- [violet](https://github.com/paullouisageneau/violet): open-source lightweight
  STUN/TURN server.
- [natcheck](https://github.com/1mb-dev/natcheck): open-source NAT behavior
  diagnosis CLI.
- [STUNner](https://github.com/l7mp/stunner): open-source Kubernetes media
  gateway for WebRTC.
- [rtpengine](https://github.com/sipwise/rtpengine): open-source RTP/media relay
  validation and SBC media-path parity.
- [RTPProxy](https://github.com/sippy/rtpproxy): open-source RTP relay and
  NAT/media-path reference.
- [erlrtpproxy](https://github.com/lemenkov/erlrtpproxy): open-source RTP
  proxy variant.
- [pylrkproxy](https://github.com/mojtabaesfandiari/pylrkproxy): open-source RTP
  proxy variant.
- [HEP / HOMER ecosystem](https://github.com/sipcapture/homer): open-source
  passive SIP/RTC capture interoperability and ladder/reporting model.
- [sngrep](https://github.com/irontec/sngrep): open-source SIP ladder
  troubleshooting reference.
- [sipgrep](https://github.com/sipcapture/sipgrep): open-source SIP packet
  sniffing and console exploration tool.
- [rtpbreak / rtpsplit](https://github.com/Naishy/rtpsplit): open-source RTP
  reconstruction and analysis reference.
- [WebRTC Troubleshooter](https://github.com/webrtc/testrtc): open-source
  client-side WebRTC diagnostics reference.
- [Trickle ICE sample](https://github.com/webrtc/samples/tree/gh-pages/src/content/peerconnection/trickle-ice):
  open-source client-side ICE/NAT debug reference.
- [tcpdump](https://github.com/the-tcpdump-group/tcpdump): open-source packet
  capture reference often used in RTC/VoIP investigations.
- [tshark / Wireshark](https://gitlab.com/wireshark/wireshark): open-source
  packet decode reference often used in RTC/VoIP investigations.

[Back to top](#awesome-rtc)

## WebRTC Servers, Gateways, And Media Apps

- [Janus Gateway](https://github.com/meetecho/janus-gateway): open-source WebRTC
  gateway and media server.
- [LiveKit](https://github.com/livekit/livekit): open-source WebRTC SFU/media
  infrastructure.
- [mediasoup](https://github.com/versatica/mediasoup): open-source WebRTC SFU
  and conferencing framework.
- [Jitsi Videobridge](https://github.com/jitsi/jitsi-videobridge) /
  [Jitsi Meet](https://github.com/jitsi/jitsi-meet): open-source WebRTC
  conferencing and SFU reference stack.
- [Kurento](https://github.com/Kurento/kurento): open-source WebRTC media
  server with media processing and recording.
- [Galene](https://github.com/jech/galene): open-source lightweight
  video-conference server.
- [OpenVidu](https://github.com/OpenVidu/openvidu): open-source
  video-conference platform built on WebRTC.
- [BigBlueButton](https://github.com/bigbluebutton/bigbluebutton): open-source
  web conferencing system.
- [MiroTalk P2P](https://github.com/miroslavpejic85/mirotalk) /
  [MiroTalk SFU](https://github.com/miroslavpejic85/mirotalksfu): open-source
  WebRTC meeting references.
- [Plug-N-Meet](https://github.com/mynaparrot/plugNmeet-server): open-source
  conferencing system built around LiveKit.
- [Medooze Media Server](https://github.com/medooze/media-server-node):
  open-source Node WebRTC media server.
- [Kraken](https://github.com/MixinNetwork/kraken): open-source Go WebRTC SFU.
- [OvenMediaEngine](https://github.com/AirenSoft/OvenMediaEngine) /
  [OvenPlayer](https://github.com/AirenSoft/OvenPlayer): open-source
  low-latency media streaming reference.
- [selkies-gstreamer](https://github.com/selkies-project/selkies-gstreamer):
  open-source low-latency Linux WebRTC and GStreamer remote desktop/media
  components.
- [Pipecat](https://github.com/pipecat-ai/pipecat): open-source voice/media
  pipeline reference.
- [VoiceBlender](https://github.com/voiceblender/voiceblender): open-source
  SIP/WebRTC/AI voice service idea source.
- [Gossipper WebRTC](https://github.com/sipcapture/gossipper): open-source
  experimental WebRTC bridge ideas.

[Back to top](#awesome-rtc)

## Practical Notes

- Choose embedded libraries when you need tight control over protocol behavior
  or application integration.
- Choose existing CLI tools and services for repeatable labs, black-box
  interoperability checks, and operational diagnostics.
- Choose full media servers, relays, and gateways when the test needs real
  media-path behavior, NAT traversal, recording, conferencing, or SFU/MCU
  semantics.

[Back to top](#awesome-rtc)
