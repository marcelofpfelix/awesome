# Awesome RTC

A curated list of open-source SIP, RTP, WebRTC, STUN/TURN, and IMS software.
media-observability software.

## SIP And VoIP User Agents

- [PJSIP / `pjsua`](https://github.com/pjsip/pjproject) [![stars/year](https://img.shields.io/github/stars/pjsip/pjproject?style=flat&color=gold&label=stars%2Fyear)](https://github.com/pjsip/pjproject) [![commits/year](https://img.shields.io/github/commit-activity/y/pjsip/pjproject?style=flat&color=blue&label=commits%2Fyear)](https://github.com/pjsip/pjproject): mature open-source
  SIP/media stack with a C API, CLI tools, NAT traversal support, and broad
  VoIP coverage.
- [liblinphone / linphone-sdk](https://gitlab.linphone.org/BC/public/linphone-sdk):
  full-featured open-source SIP/VoIP SDK and client stack.
- [`linphonec`](https://gitlab.linphone.org/BC/public/linphone-sdk): liblinphone
  console client, useful as a command/control and callback reference for call
  state, auth, DTMF, text, auto-answer, and daemon-style command handling.
- [baresip](https://github.com/baresip/baresip) [![stars/year](https://img.shields.io/github/stars/baresip/baresip?style=flat&color=gold&label=stars%2Fyear)](https://github.com/baresip/baresip) [![commits/year](https://img.shields.io/github/commit-activity/y/baresip/baresip?style=flat&color=blue&label=commits%2Fyear)](https://github.com/baresip/baresip): lightweight open-source SIP
  softphone stack and automation reference.
- [MicroSIP](https://github.com/MicroSIP/MicroSIP) [![stars/year](https://img.shields.io/github/stars/MicroSIP/MicroSIP?style=flat&color=gold&label=stars%2Fyear)](https://github.com/MicroSIP/MicroSIP) [![commits/year](https://img.shields.io/github/commit-activity/y/MicroSIP/MicroSIP?style=flat&color=blue&label=commits%2Fyear)](https://github.com/MicroSIP/MicroSIP): open-source Windows SIP
  softphone based on PJSIP.
- [CSipSimple](https://github.com/r3gis3r/CSipSimple) [![stars/year](https://img.shields.io/github/stars/r3gis3r/CSipSimple?style=flat&color=gold&label=stars%2Fyear)](https://github.com/r3gis3r/CSipSimple) [![commits/year](https://img.shields.io/github/commit-activity/y/r3gis3r/CSipSimple?style=flat&color=blue&label=commits%2Fyear)](https://github.com/r3gis3r/CSipSimple): open-source Android SIP
  softphone history and SIP/NAT behavior reference.
- [Jitsi Desktop](https://github.com/jitsi/jitsi) [![stars/year](https://img.shields.io/github/stars/jitsi/jitsi?style=flat&color=gold&label=stars%2Fyear)](https://github.com/jitsi/jitsi) [![commits/year](https://img.shields.io/github/commit-activity/y/jitsi/jitsi?style=flat&color=blue&label=commits%2Fyear)](https://github.com/jitsi/jitsi): open-source desktop SIP/XMPP
  softphone reference.
- [Twinkle](https://github.com/LubosD/twinkle) [![stars/year](https://img.shields.io/github/stars/LubosD/twinkle?style=flat&color=gold&label=stars%2Fyear)](https://github.com/LubosD/twinkle) [![commits/year](https://img.shields.io/github/commit-activity/y/LubosD/twinkle?style=flat&color=blue&label=commits%2Fyear)](https://github.com/LubosD/twinkle): open-source Linux SIP softphone
  reference.
- [diago](https://github.com/emiago/diago) [![stars/year](https://img.shields.io/github/stars/emiago/diago?style=flat&color=gold&label=stars%2Fyear)](https://github.com/emiago/diago) [![commits/year](https://img.shields.io/github/commit-activity/y/emiago/diago?style=flat&color=blue&label=commits%2Fyear)](https://github.com/emiago/diago) /
  [sipgo](https://github.com/emiago/sipgo) [![stars/year](https://img.shields.io/github/stars/emiago/sipgo?style=flat&color=gold&label=stars%2Fyear)](https://github.com/emiago/sipgo) [![commits/year](https://img.shields.io/github/commit-activity/y/emiago/sipgo?style=flat&color=blue&label=commits%2Fyear)](https://github.com/emiago/sipgo): open-source Go references for SIP
  dialogs, RTP, DTMF, WAV, and media helpers.

[Back to top](#awesome-rtc)

## SIP Servers, PBX, Proxies, And B2BUA

- [Kamailio](https://github.com/kamailio/kamailio) [![stars/year](https://img.shields.io/github/stars/kamailio/kamailio?style=flat&color=gold&label=stars%2Fyear)](https://github.com/kamailio/kamailio) [![commits/year](https://img.shields.io/github/commit-activity/y/kamailio/kamailio?style=flat&color=blue&label=commits%2Fyear)](https://github.com/kamailio/kamailio): open-source SIP
  proxy/SBC/lab service and module-architecture reference.
- [OpenSIPS](https://github.com/OpenSIPS/opensips) [![stars/year](https://img.shields.io/github/stars/OpenSIPS/opensips?style=flat&color=gold&label=stars%2Fyear)](https://github.com/OpenSIPS/opensips) [![commits/year](https://img.shields.io/github/commit-activity/y/OpenSIPS/opensips?style=flat&color=blue&label=commits%2Fyear)](https://github.com/OpenSIPS/opensips): open-source SIP
  proxy/server and carrier-routing reference.
- [Asterisk](https://github.com/asterisk/asterisk) [![stars/year](https://img.shields.io/github/stars/asterisk/asterisk?style=flat&color=gold&label=stars%2Fyear)](https://github.com/asterisk/asterisk) [![commits/year](https://img.shields.io/github/commit-activity/y/asterisk/asterisk?style=flat&color=blue&label=commits%2Fyear)](https://github.com/asterisk/asterisk): open-source PBX and
  telephony application framework.
- [FreeSWITCH](https://github.com/signalwire/freeswitch) [![stars/year](https://img.shields.io/github/stars/signalwire/freeswitch?style=flat&color=gold&label=stars%2Fyear)](https://github.com/signalwire/freeswitch) [![commits/year](https://img.shields.io/github/commit-activity/y/signalwire/freeswitch?style=flat&color=blue&label=commits%2Fyear)](https://github.com/signalwire/freeswitch): open-source PBX/media
  service for complex call-control and media scenarios.
- [Flexisip](https://gitlab.linphone.org/BC/public/flexisip): open-source SIP
  proxy, presence, and group-chat suite from Belledonne.
- [drachtio](https://github.com/drachtio/drachtio-server) [![stars/year](https://img.shields.io/github/stars/drachtio/drachtio-server?style=flat&color=gold&label=stars%2Fyear)](https://github.com/drachtio/drachtio-server) [![commits/year](https://img.shields.io/github/commit-activity/y/drachtio/drachtio-server?style=flat&color=blue&label=commits%2Fyear)](https://github.com/drachtio/drachtio-server): open-source SIP
  server framework for Node.js applications.
- [reSIProcate / Repro](https://github.com/resiprocate/resiprocate) [![stars/year](https://img.shields.io/github/stars/resiprocate/resiprocate?style=flat&color=gold&label=stars%2Fyear)](https://github.com/resiprocate/resiprocate) [![commits/year](https://img.shields.io/github/commit-activity/y/resiprocate/resiprocate?style=flat&color=blue&label=commits%2Fyear)](https://github.com/resiprocate/resiprocate): open-source
  SIP stack and federated SIP server.
- [Routr](https://github.com/fonoster/routr) [![stars/year](https://img.shields.io/github/stars/fonoster/routr?style=flat&color=gold&label=stars%2Fyear)](https://github.com/fonoster/routr) [![commits/year](https://img.shields.io/github/commit-activity/y/fonoster/routr?style=flat&color=blue&label=commits%2Fyear)](https://github.com/fonoster/routr): open-source lightweight SIP proxy,
  location server, and registrar.
- [Sippy B2BUA](https://github.com/sippy/b2bua) [![stars/year](https://img.shields.io/github/stars/sippy/b2bua?style=flat&color=gold&label=stars%2Fyear)](https://github.com/sippy/b2bua) [![commits/year](https://img.shields.io/github/commit-activity/y/sippy/b2bua?style=flat&color=blue&label=commits%2Fyear)](https://github.com/sippy/b2bua): open-source Python
  back-to-back user-agent server.
- [Sippy Go B2BUA](https://github.com/sippy/go-b2bua) [![stars/year](https://img.shields.io/github/stars/sippy/go-b2bua?style=flat&color=gold&label=stars%2Fyear)](https://github.com/sippy/go-b2bua) [![commits/year](https://img.shields.io/github/commit-activity/y/sippy/go-b2bua?style=flat&color=blue&label=commits%2Fyear)](https://github.com/sippy/go-b2bua): open-source Go
  back-to-back user-agent server.
- [SEMS](https://github.com/sems-server/sems) [![stars/year](https://img.shields.io/github/stars/sems-server/sems?style=flat&color=gold&label=stars%2Fyear)](https://github.com/sems-server/sems) [![commits/year](https://img.shields.io/github/commit-activity/y/sems-server/sems?style=flat&color=blue&label=commits%2Fyear)](https://github.com/sems-server/sems): open-source SIP media and
  application server.
- [Siproxd](https://sourceforge.net/projects/siproxd/): open-source SIP
  proxy/masquerading daemon.
- [Dubango WebRTC2SIP](https://github.com/DoubangoTelecom/webrtc2sip) [![stars/year](https://img.shields.io/github/stars/DoubangoTelecom/webrtc2sip?style=flat&color=gold&label=stars%2Fyear)](https://github.com/DoubangoTelecom/webrtc2sip) [![commits/year](https://img.shields.io/github/commit-activity/y/DoubangoTelecom/webrtc2sip?style=flat&color=blue&label=commits%2Fyear)](https://github.com/DoubangoTelecom/webrtc2sip):
  open-source SIP/WebRTC gateway reference.
- [Kazoo](https://github.com/2600hz/kazoo) [![stars/year](https://img.shields.io/github/stars/2600hz/kazoo?style=flat&color=gold&label=stars%2Fyear)](https://github.com/2600hz/kazoo) [![commits/year](https://img.shields.io/github/commit-activity/y/2600hz/kazoo?style=flat&color=blue&label=commits%2Fyear)](https://github.com/2600hz/kazoo): open-source carrier VoIP API
  platform built around FreeSWITCH and Kamailio.
- [Wazo](https://github.com/wazo-platform/wazo-platform) [![stars/year](https://img.shields.io/github/stars/wazo-platform/wazo-platform?style=flat&color=gold&label=stars%2Fyear)](https://github.com/wazo-platform/wazo-platform) [![commits/year](https://img.shields.io/github/commit-activity/y/wazo-platform/wazo-platform?style=flat&color=blue&label=commits%2Fyear)](https://github.com/wazo-platform/wazo-platform): open-source VoIP API
  platform built around Asterisk, Kamailio, and RTPEngine.
- [FusionPBX](https://github.com/fusionpbx/fusionpbx) [![stars/year](https://img.shields.io/github/stars/fusionpbx/fusionpbx?style=flat&color=gold&label=stars%2Fyear)](https://github.com/fusionpbx/fusionpbx) [![commits/year](https://img.shields.io/github/commit-activity/y/fusionpbx/fusionpbx?style=flat&color=blue&label=commits%2Fyear)](https://github.com/fusionpbx/fusionpbx): open-source FreeSWITCH
  web management and multitenant PBX system.
- [FreePBX](https://github.com/FreePBX/framework) [![stars/year](https://img.shields.io/github/stars/FreePBX/framework?style=flat&color=gold&label=stars%2Fyear)](https://github.com/FreePBX/framework) [![commits/year](https://img.shields.io/github/commit-activity/y/FreePBX/framework?style=flat&color=blue&label=commits%2Fyear)](https://github.com/FreePBX/framework): open-source Asterisk web
  management system.
- [Fonoster](https://github.com/fonoster/fonoster) [![stars/year](https://img.shields.io/github/stars/fonoster/fonoster?style=flat&color=gold&label=stars%2Fyear)](https://github.com/fonoster/fonoster) [![commits/year](https://img.shields.io/github/commit-activity/y/fonoster/fonoster?style=flat&color=blue&label=commits%2Fyear)](https://github.com/fonoster/fonoster): open-source programmable
  telecom stack.
- [jambonz](https://github.com/jambonz/jambonz-feature-server) [![stars/year](https://img.shields.io/github/stars/jambonz/jambonz-feature-server?style=flat&color=gold&label=stars%2Fyear)](https://github.com/jambonz/jambonz-feature-server) [![commits/year](https://img.shields.io/github/commit-activity/y/jambonz/jambonz-feature-server?style=flat&color=blue&label=commits%2Fyear)](https://github.com/jambonz/jambonz-feature-server): open-source
  CPaaS for SIP and programmable voice.
- [IVOZ Provider](https://github.com/irontec/ivozprovider) [![stars/year](https://img.shields.io/github/stars/irontec/ivozprovider?style=flat&color=gold&label=stars%2Fyear)](https://github.com/irontec/ivozprovider) [![commits/year](https://img.shields.io/github/commit-activity/y/irontec/ivozprovider?style=flat&color=blue&label=commits%2Fyear)](https://github.com/irontec/ivozprovider): open-source
  multitenant VoIP provider platform.
- [CGRateS](https://github.com/cgrates/cgrates) [![stars/year](https://img.shields.io/github/stars/cgrates/cgrates?style=flat&color=gold&label=stars%2Fyear)](https://github.com/cgrates/cgrates) [![commits/year](https://img.shields.io/github/commit-activity/y/cgrates/cgrates?style=flat&color=blue&label=commits%2Fyear)](https://github.com/cgrates/cgrates): open-source carrier-grade
  rating and charging server.

[Back to top](#awesome-rtc)

## SIP Scenario And Load Tools

- [SIPp](https://github.com/SIPp/sipp) [![stars/year](https://img.shields.io/github/stars/SIPp/sipp?style=flat&color=gold&label=stars%2Fyear)](https://github.com/SIPp/sipp) [![commits/year](https://img.shields.io/github/commit-activity/y/SIPp/sipp?style=flat&color=blue&label=commits%2Fyear)](https://github.com/SIPp/sipp): canonical open-source SIP scenario and
  load-generation tool with XML scenarios, CSV injection, rate controls, and
  trace/stat artifacts.
- [Gossipper](https://github.com/sipcapture/gossipper) [![stars/year](https://img.shields.io/github/stars/sipcapture/gossipper?style=flat&color=gold&label=stars%2Fyear)](https://github.com/sipcapture/gossipper) [![commits/year](https://img.shields.io/github/commit-activity/y/sipcapture/gossipper?style=flat&color=blue&label=commits%2Fyear)](https://github.com/sipcapture/gossipper): open-source
  SIPp-compatible Go platform with RTP, HEP, reporting, and PCAP-to-scenario
  ideas.
- [sipexer](https://github.com/miconda/sipexer) [![stars/year](https://img.shields.io/github/stars/miconda/sipexer?style=flat&color=gold&label=stars%2Fyear)](https://github.com/miconda/sipexer) [![commits/year](https://img.shields.io/github/commit-activity/y/miconda/sipexer?style=flat&color=blue&label=commits%2Fyear)](https://github.com/miconda/sipexer): open-source focused SIP CLI
  for OPTIONS, REGISTER, MESSAGE, INVITE, authentication, and transports.
- [sipsak](https://github.com/nils-ohlmeier/sipsak) [![stars/year](https://img.shields.io/github/stars/nils-ohlmeier/sipsak?style=flat&color=gold&label=stars%2Fyear)](https://github.com/nils-ohlmeier/sipsak) [![commits/year](https://img.shields.io/github/commit-activity/y/nils-ohlmeier/sipsak?style=flat&color=blue&label=commits%2Fyear)](https://github.com/nils-ohlmeier/sipsak): open-source legacy SIP
  diagnostics.
- [SIPVicious](https://github.com/EnableSecurity/sipvicious) [![stars/year](https://img.shields.io/github/stars/EnableSecurity/sipvicious?style=flat&color=gold&label=stars%2Fyear)](https://github.com/EnableSecurity/sipvicious) [![commits/year](https://img.shields.io/github/commit-activity/y/EnableSecurity/sipvicious?style=flat&color=blue&label=commits%2Fyear)](https://github.com/EnableSecurity/sipvicious): open-source SIP
  security audit suite.
- [SIPPTS](https://github.com/Pepelux/sippts) [![stars/year](https://img.shields.io/github/stars/Pepelux/sippts?style=flat&color=gold&label=stars%2Fyear)](https://github.com/Pepelux/sippts) [![commits/year](https://img.shields.io/github/commit-activity/y/Pepelux/sippts?style=flat&color=blue&label=commits%2Fyear)](https://github.com/Pepelux/sippts): open-source SIP
  penetration-testing and protocol test toolkit.
- [sipcmd](https://github.com/tmakkonen/sipcmd) [![stars/year](https://img.shields.io/github/stars/tmakkonen/sipcmd?style=flat&color=gold&label=stars%2Fyear)](https://github.com/tmakkonen/sipcmd) [![commits/year](https://img.shields.io/github/commit-activity/y/tmakkonen/sipcmd?style=flat&color=blue&label=commits%2Fyear)](https://github.com/tmakkonen/sipcmd) /
  [sipcmd2](https://github.com/guisousanunes/sipcmd2) [![stars/year](https://img.shields.io/github/stars/guisousanunes/sipcmd2?style=flat&color=gold&label=stars%2Fyear)](https://github.com/guisousanunes/sipcmd2) [![commits/year](https://img.shields.io/github/commit-activity/y/guisousanunes/sipcmd2?style=flat&color=blue&label=commits%2Fyear)](https://github.com/guisousanunes/sipcmd2): open-source command-line
  SIP call tools.
- [telefonist](https://github.com/negbie/telefonist) [![stars/year](https://img.shields.io/github/stars/negbie/telefonist?style=flat&color=gold&label=stars%2Fyear)](https://github.com/negbie/telefonist) [![commits/year](https://img.shields.io/github/commit-activity/y/negbie/telefonist?style=flat&color=blue&label=commits%2Fyear)](https://github.com/negbie/telefonist): open-source SIP
  automation reference.
- [wsctl](https://github.com/kamailio/kamailio/tree/master/misc/tools/wsctl) [![stars/year](https://img.shields.io/github/stars/kamailio/kamailio?style=flat&color=gold&label=stars%2Fyear)](https://github.com/kamailio/kamailio/tree/master/misc/tools/wsctl) [![commits/year](https://img.shields.io/github/commit-activity/y/kamailio/kamailio?style=flat&color=blue&label=commits%2Fyear)](https://github.com/kamailio/kamailio/tree/master/misc/tools/wsctl):
  open-source WebSocket command-line tool from the Kamailio ecosystem.
- [protos-sip](https://gitlab.com/kalilinux/packages/protos-sip): open-source SIP
  protocol test source package.
- [protoshoot](https://github.com/kamailio/kamailio/tree/master/misc/tools/protoshoot) [![stars/year](https://img.shields.io/github/stars/kamailio/kamailio?style=flat&color=gold&label=stars%2Fyear)](https://github.com/kamailio/kamailio/tree/master/misc/tools/protoshoot) [![commits/year](https://img.shields.io/github/commit-activity/y/kamailio/kamailio?style=flat&color=blue&label=commits%2Fyear)](https://github.com/kamailio/kamailio/tree/master/misc/tools/protoshoot):
  open-source raw-message shooting idea source from the Kamailio tree.

[Back to top](#awesome-rtc)

## SIP, RTP, And WebRTC Libraries

- [PJSIP / PJPROJECT](https://github.com/pjsip/pjproject) [![stars/year](https://img.shields.io/github/stars/pjsip/pjproject?style=flat&color=gold&label=stars%2Fyear)](https://github.com/pjsip/pjproject) [![commits/year](https://img.shields.io/github/commit-activity/y/pjsip/pjproject?style=flat&color=blue&label=commits%2Fyear)](https://github.com/pjsip/pjproject): open-source C SIP,
  media, and NAT traversal stack.
- [liblinphone / linphone-sdk](https://gitlab.linphone.org/BC/public/linphone-sdk):
  open-source SIP/VoIP SDK and full client stack.
- [libre](https://github.com/baresip/re) [![stars/year](https://img.shields.io/github/stars/baresip/re?style=flat&color=gold&label=stars%2Fyear)](https://github.com/baresip/re) [![commits/year](https://img.shields.io/github/commit-activity/y/baresip/re?style=flat&color=blue&label=commits%2Fyear)](https://github.com/baresip/re) /
  [librem](https://github.com/baresip/rem) [![stars/year](https://img.shields.io/github/stars/baresip/rem?style=flat&color=gold&label=stars%2Fyear)](https://github.com/baresip/rem) [![commits/year](https://img.shields.io/github/commit-activity/y/baresip/rem?style=flat&color=blue&label=commits%2Fyear)](https://github.com/baresip/rem) /
  [baresip](https://github.com/baresip/baresip) [![stars/year](https://img.shields.io/github/stars/baresip/baresip?style=flat&color=gold&label=stars%2Fyear)](https://github.com/baresip/baresip) [![commits/year](https://img.shields.io/github/commit-activity/y/baresip/baresip?style=flat&color=blue&label=commits%2Fyear)](https://github.com/baresip/baresip): open-source SIP, SDP,
  RTP/RTCP, STUN, TURN, ICE, and user-agent building blocks.
- [oSIP](https://git.savannah.gnu.org/cgit/osip.git) /
  [eXosip](https://git.savannah.nongnu.org/cgit/exosip.git): open-source C SIP
  libraries for parser/dialog/user-agent primitives.
- [Sofia-SIP](https://github.com/freeswitch/sofia-sip) [![stars/year](https://img.shields.io/github/stars/freeswitch/sofia-sip?style=flat&color=gold&label=stars%2Fyear)](https://github.com/freeswitch/sofia-sip) [![commits/year](https://img.shields.io/github/commit-activity/y/freeswitch/sofia-sip?style=flat&color=blue&label=commits%2Fyear)](https://github.com/freeswitch/sofia-sip): open-source C SIP
  library used by FreeSWITCH.
- [reSIProcate](https://github.com/resiprocate/resiprocate) [![stars/year](https://img.shields.io/github/stars/resiprocate/resiprocate?style=flat&color=gold&label=stars%2Fyear)](https://github.com/resiprocate/resiprocate) [![commits/year](https://img.shields.io/github/commit-activity/y/resiprocate/resiprocate?style=flat&color=blue&label=commits%2Fyear)](https://github.com/resiprocate/resiprocate): open-source C++
  SIP stack.
- [JAIN-SIP](https://github.com/usnistgov/jsip) [![stars/year](https://img.shields.io/github/stars/usnistgov/jsip?style=flat&color=gold&label=stars%2Fyear)](https://github.com/usnistgov/jsip) [![commits/year](https://img.shields.io/github/commit-activity/y/usnistgov/jsip?style=flat&color=blue&label=commits%2Fyear)](https://github.com/usnistgov/jsip): open-source Java SIP stack.
- [sipsorcery](https://github.com/sipsorcery-org/sipsorcery) [![stars/year](https://img.shields.io/github/stars/sipsorcery-org/sipsorcery?style=flat&color=gold&label=stars%2Fyear)](https://github.com/sipsorcery-org/sipsorcery) [![commits/year](https://img.shields.io/github/commit-activity/y/sipsorcery-org/sipsorcery?style=flat&color=blue&label=commits%2Fyear)](https://github.com/sipsorcery-org/sipsorcery): open-source .NET
  SIP, SDP, RTP, STUN, and WebRTC stack.
- [JsSIP](https://github.com/versatica/JsSIP) [![stars/year](https://img.shields.io/github/stars/versatica/JsSIP?style=flat&color=gold&label=stars%2Fyear)](https://github.com/versatica/JsSIP) [![commits/year](https://img.shields.io/github/commit-activity/y/versatica/JsSIP?style=flat&color=blue&label=commits%2Fyear)](https://github.com/versatica/JsSIP): open-source JavaScript
  SIP-over-WebSocket library.
- [SIP.js](https://github.com/onsip/SIP.js) [![stars/year](https://img.shields.io/github/stars/onsip/SIP.js?style=flat&color=gold&label=stars%2Fyear)](https://github.com/onsip/SIP.js) [![commits/year](https://img.shields.io/github/commit-activity/y/onsip/SIP.js?style=flat&color=blue&label=commits%2Fyear)](https://github.com/onsip/SIP.js): open-source JavaScript SIP
  signaling library.
- [sipML5](https://github.com/DoubangoTelecom/sipml5) [![stars/year](https://img.shields.io/github/stars/DoubangoTelecom/sipml5?style=flat&color=gold&label=stars%2Fyear)](https://github.com/DoubangoTelecom/sipml5) [![commits/year](https://img.shields.io/github/commit-activity/y/DoubangoTelecom/sipml5?style=flat&color=blue&label=commits%2Fyear)](https://github.com/DoubangoTelecom/sipml5) /
  [sipML5-NG](https://github.com/cloudonix/sipml5-ng) [![stars/year](https://img.shields.io/github/stars/cloudonix/sipml5-ng?style=flat&color=gold&label=stars%2Fyear)](https://github.com/cloudonix/sipml5-ng) [![commits/year](https://img.shields.io/github/commit-activity/y/cloudonix/sipml5-ng?style=flat&color=blue&label=commits%2Fyear)](https://github.com/cloudonix/sipml5-ng): open-source browser
  SIP/WebRTC client references.
- [dart-sip-ua](https://github.com/flutter-webrtc/dart-sip-ua) [![stars/year](https://img.shields.io/github/stars/flutter-webrtc/dart-sip-ua?style=flat&color=gold&label=stars%2Fyear)](https://github.com/flutter-webrtc/dart-sip-ua) [![commits/year](https://img.shields.io/github/commit-activity/y/flutter-webrtc/dart-sip-ua?style=flat&color=blue&label=commits%2Fyear)](https://github.com/flutter-webrtc/dart-sip-ua): open-source
  Dart port of JsSIP.
- [RTCKit/PHP SIP](https://github.com/rtckit/php-sip) [![stars/year](https://img.shields.io/github/stars/rtckit/php-sip?style=flat&color=gold&label=stars%2Fyear)](https://github.com/rtckit/php-sip) [![commits/year](https://img.shields.io/github/commit-activity/y/rtckit/php-sip?style=flat&color=blue&label=commits%2Fyear)](https://github.com/rtckit/php-sip): open-source PHP SIP
  parser and renderer.
- [rsip](https://github.com/Televiska/rsip) [![stars/year](https://img.shields.io/github/stars/Televiska/rsip?style=flat&color=gold&label=stars%2Fyear)](https://github.com/Televiska/rsip) [![commits/year](https://img.shields.io/github/commit-activity/y/Televiska/rsip?style=flat&color=blue&label=commits%2Fyear)](https://github.com/Televiska/rsip): open-source Rust SIP parser/model
  reference.
- [sipcore](https://github.com/kurotych/sipcore) [![stars/year](https://img.shields.io/github/stars/kurotych/sipcore?style=flat&color=gold&label=stars%2Fyear)](https://github.com/kurotych/sipcore) [![commits/year](https://img.shields.io/github/commit-activity/y/kurotych/sipcore?style=flat&color=blue&label=commits%2Fyear)](https://github.com/kurotych/sipcore): open-source Rust SIP
  implementation idea.
- [libsip](https://github.com/ByteHeathen/libsip) [![stars/year](https://img.shields.io/github/stars/ByteHeathen/libsip?style=flat&color=gold&label=stars%2Fyear)](https://github.com/ByteHeathen/libsip) [![commits/year](https://img.shields.io/github/commit-activity/y/ByteHeathen/libsip?style=flat&color=blue&label=commits%2Fyear)](https://github.com/ByteHeathen/libsip): open-source Rust SIP
  implementation idea.
- [parsip](https://github.com/kamarkiewicz/parsip) [![stars/year](https://img.shields.io/github/stars/kamarkiewicz/parsip?style=flat&color=gold&label=stars%2Fyear)](https://github.com/kamarkiewicz/parsip) [![commits/year](https://img.shields.io/github/commit-activity/y/kamarkiewicz/parsip?style=flat&color=blue&label=commits%2Fyear)](https://github.com/kamarkiewicz/parsip): open-source Rust SIP parser
  implementation idea.
- [pyVoIP](https://github.com/tayler6000/pyVoIP) [![stars/year](https://img.shields.io/github/stars/tayler6000/pyVoIP?style=flat&color=gold&label=stars%2Fyear)](https://github.com/tayler6000/pyVoIP) [![commits/year](https://img.shields.io/github/commit-activity/y/tayler6000/pyVoIP?style=flat&color=blue&label=commits%2Fyear)](https://github.com/tayler6000/pyVoIP): open-source Python VoIP
  library.
- [ersip](https://github.com/poroh/ersip) [![stars/year](https://img.shields.io/github/stars/poroh/ersip?style=flat&color=gold&label=stars%2Fyear)](https://github.com/poroh/ersip) [![commits/year](https://img.shields.io/github/commit-activity/y/poroh/ersip?style=flat&color=blue&label=commits%2Fyear)](https://github.com/poroh/ersip) /
  [NkSIP](https://github.com/NetComposer/nksip) [![stars/year](https://img.shields.io/github/stars/NetComposer/nksip?style=flat&color=gold&label=stars%2Fyear)](https://github.com/NetComposer/nksip) [![commits/year](https://img.shields.io/github/commit-activity/y/NetComposer/nksip?style=flat&color=blue&label=commits%2Fyear)](https://github.com/NetComposer/nksip): open-source Erlang SIP
  building blocks.
- [Pion WebRTC](https://github.com/pion/webrtc) [![stars/year](https://img.shields.io/github/stars/pion/webrtc?style=flat&color=gold&label=stars%2Fyear)](https://github.com/pion/webrtc) [![commits/year](https://img.shields.io/github/commit-activity/y/pion/webrtc?style=flat&color=blue&label=commits%2Fyear)](https://github.com/pion/webrtc): open-source Go WebRTC stack.
- [Pion TURN](https://github.com/pion/turn) [![stars/year](https://img.shields.io/github/stars/pion/turn?style=flat&color=gold&label=stars%2Fyear)](https://github.com/pion/turn) [![commits/year](https://img.shields.io/github/commit-activity/y/pion/turn?style=flat&color=blue&label=commits%2Fyear)](https://github.com/pion/turn): open-source Go TURN toolkit.
- [aiortc](https://github.com/aiortc/aiortc) [![stars/year](https://img.shields.io/github/stars/aiortc/aiortc?style=flat&color=gold&label=stars%2Fyear)](https://github.com/aiortc/aiortc) [![commits/year](https://img.shields.io/github/commit-activity/y/aiortc/aiortc?style=flat&color=blue&label=commits%2Fyear)](https://github.com/aiortc/aiortc): open-source Python WebRTC
  behavior reference.
- [libdatachannel](https://github.com/paullouisageneau/libdatachannel) [![stars/year](https://img.shields.io/github/stars/paullouisageneau/libdatachannel?style=flat&color=gold&label=stars%2Fyear)](https://github.com/paullouisageneau/libdatachannel) [![commits/year](https://img.shields.io/github/commit-activity/y/paullouisageneau/libdatachannel?style=flat&color=blue&label=commits%2Fyear)](https://github.com/paullouisageneau/libdatachannel):
  open-source C++ WebRTC data-channel and media-transport library.
- [datachannel-wasm](https://github.com/paullouisageneau/datachannel-wasm) [![stars/year](https://img.shields.io/github/stars/paullouisageneau/datachannel-wasm?style=flat&color=gold&label=stars%2Fyear)](https://github.com/paullouisageneau/datachannel-wasm) [![commits/year](https://img.shields.io/github/commit-activity/y/paullouisageneau/datachannel-wasm?style=flat&color=blue&label=commits%2Fyear)](https://github.com/paullouisageneau/datachannel-wasm):
  open-source WebAssembly build of libdatachannel.
- [rawrtc](https://github.com/rawrtc/rawrtc) [![stars/year](https://img.shields.io/github/stars/rawrtc/rawrtc?style=flat&color=gold&label=stars%2Fyear)](https://github.com/rawrtc/rawrtc) [![commits/year](https://img.shields.io/github/commit-activity/y/rawrtc/rawrtc?style=flat&color=blue&label=commits%2Fyear)](https://github.com/rawrtc/rawrtc): open-source WebRTC/ORTC C
  library.
- [werift](https://github.com/shinyoshiaki/werift-webrtc) [![stars/year](https://img.shields.io/github/stars/shinyoshiaki/werift-webrtc?style=flat&color=gold&label=stars%2Fyear)](https://github.com/shinyoshiaki/werift-webrtc) [![commits/year](https://img.shields.io/github/commit-activity/y/shinyoshiaki/werift-webrtc?style=flat&color=blue&label=commits%2Fyear)](https://github.com/shinyoshiaki/werift-webrtc): open-source
  TypeScript WebRTC implementation.
- [node-datachannel](https://github.com/murat-dogan/node-datachannel) [![stars/year](https://img.shields.io/github/stars/murat-dogan/node-datachannel?style=flat&color=gold&label=stars%2Fyear)](https://github.com/murat-dogan/node-datachannel) [![commits/year](https://img.shields.io/github/commit-activity/y/murat-dogan/node-datachannel?style=flat&color=blue&label=commits%2Fyear)](https://github.com/murat-dogan/node-datachannel):
  open-source Node bindings for libdatachannel.
- [node-webrtc](https://github.com/node-webrtc/node-webrtc) [![stars/year](https://img.shields.io/github/stars/node-webrtc/node-webrtc?style=flat&color=gold&label=stars%2Fyear)](https://github.com/node-webrtc/node-webrtc) [![commits/year](https://img.shields.io/github/commit-activity/y/node-webrtc/node-webrtc?style=flat&color=blue&label=commits%2Fyear)](https://github.com/node-webrtc/node-webrtc): open-source Node
  bindings for WebRTC.
- [rtcrs/webrtc](https://github.com/rtcrs/webrtc) [![stars/year](https://img.shields.io/github/stars/rtcrs/webrtc?style=flat&color=gold&label=stars%2Fyear)](https://github.com/rtcrs/webrtc) [![commits/year](https://img.shields.io/github/commit-activity/y/rtcrs/webrtc?style=flat&color=blue&label=commits%2Fyear)](https://github.com/rtcrs/webrtc): open-source Rust WebRTC
  stack.

[Back to top](#awesome-rtc)

## Network, Media, NAT, And Observability

- [STUNTMAN](https://github.com/jselbie/stunserver) [![stars/year](https://img.shields.io/github/stars/jselbie/stunserver?style=flat&color=gold&label=stars%2Fyear)](https://github.com/jselbie/stunserver) [![commits/year](https://img.shields.io/github/commit-activity/y/jselbie/stunserver?style=flat&color=blue&label=commits%2Fyear)](https://github.com/jselbie/stunserver): open-source STUN/NAT
  behavior checks through `stunclient` and a fixture server.
- [coturn](https://github.com/coturn/coturn) [![stars/year](https://img.shields.io/github/stars/coturn/coturn?style=flat&color=gold&label=stars%2Fyear)](https://github.com/coturn/coturn) [![commits/year](https://img.shields.io/github/commit-activity/y/coturn/coturn?style=flat&color=blue&label=commits%2Fyear)](https://github.com/coturn/coturn): open-source TURN/STUN server and
  common VoIP/WebRTC lab dependency for TURN allocation, relay, auth, TLS, and
  DTLS validation.
- [eturnal](https://github.com/processone/eturnal) [![stars/year](https://img.shields.io/github/stars/processone/eturnal?style=flat&color=gold&label=stars%2Fyear)](https://github.com/processone/eturnal) [![commits/year](https://img.shields.io/github/commit-activity/y/processone/eturnal?style=flat&color=blue&label=commits%2Fyear)](https://github.com/processone/eturnal): open-source Erlang
  STUN/TURN server.
- [turn-rs](https://github.com/mycrl/turn-rs) [![stars/year](https://img.shields.io/github/stars/mycrl/turn-rs?style=flat&color=gold&label=stars%2Fyear)](https://github.com/mycrl/turn-rs) [![commits/year](https://img.shields.io/github/commit-activity/y/mycrl/turn-rs?style=flat&color=blue&label=commits%2Fyear)](https://github.com/mycrl/turn-rs): open-source Rust TURN server.
- [violet](https://github.com/paullouisageneau/violet) [![stars/year](https://img.shields.io/github/stars/paullouisageneau/violet?style=flat&color=gold&label=stars%2Fyear)](https://github.com/paullouisageneau/violet) [![commits/year](https://img.shields.io/github/commit-activity/y/paullouisageneau/violet?style=flat&color=blue&label=commits%2Fyear)](https://github.com/paullouisageneau/violet): open-source lightweight
  STUN/TURN server.
- [natcheck](https://github.com/1mb-dev/natcheck) [![stars/year](https://img.shields.io/github/stars/1mb-dev/natcheck?style=flat&color=gold&label=stars%2Fyear)](https://github.com/1mb-dev/natcheck) [![commits/year](https://img.shields.io/github/commit-activity/y/1mb-dev/natcheck?style=flat&color=blue&label=commits%2Fyear)](https://github.com/1mb-dev/natcheck): open-source NAT behavior
  diagnosis CLI.
- [STUNner](https://github.com/l7mp/stunner) [![stars/year](https://img.shields.io/github/stars/l7mp/stunner?style=flat&color=gold&label=stars%2Fyear)](https://github.com/l7mp/stunner) [![commits/year](https://img.shields.io/github/commit-activity/y/l7mp/stunner?style=flat&color=blue&label=commits%2Fyear)](https://github.com/l7mp/stunner): open-source Kubernetes media
  gateway for WebRTC.
- [rtpengine](https://github.com/sipwise/rtpengine) [![stars/year](https://img.shields.io/github/stars/sipwise/rtpengine?style=flat&color=gold&label=stars%2Fyear)](https://github.com/sipwise/rtpengine) [![commits/year](https://img.shields.io/github/commit-activity/y/sipwise/rtpengine?style=flat&color=blue&label=commits%2Fyear)](https://github.com/sipwise/rtpengine): open-source RTP/media relay
  validation and SBC media-path parity.
- [RTPProxy](https://github.com/sippy/rtpproxy) [![stars/year](https://img.shields.io/github/stars/sippy/rtpproxy?style=flat&color=gold&label=stars%2Fyear)](https://github.com/sippy/rtpproxy) [![commits/year](https://img.shields.io/github/commit-activity/y/sippy/rtpproxy?style=flat&color=blue&label=commits%2Fyear)](https://github.com/sippy/rtpproxy): open-source RTP relay and
  NAT/media-path reference.
- [erlrtpproxy](https://github.com/lemenkov/erlrtpproxy) [![stars/year](https://img.shields.io/github/stars/lemenkov/erlrtpproxy?style=flat&color=gold&label=stars%2Fyear)](https://github.com/lemenkov/erlrtpproxy) [![commits/year](https://img.shields.io/github/commit-activity/y/lemenkov/erlrtpproxy?style=flat&color=blue&label=commits%2Fyear)](https://github.com/lemenkov/erlrtpproxy): open-source RTP
  proxy variant.
- [pylrkproxy](https://github.com/mojtabaesfandiari/pylrkproxy) [![stars/year](https://img.shields.io/github/stars/mojtabaesfandiari/pylrkproxy?style=flat&color=gold&label=stars%2Fyear)](https://github.com/mojtabaesfandiari/pylrkproxy) [![commits/year](https://img.shields.io/github/commit-activity/y/mojtabaesfandiari/pylrkproxy?style=flat&color=blue&label=commits%2Fyear)](https://github.com/mojtabaesfandiari/pylrkproxy): open-source RTP
  proxy variant.
- [HEP / HOMER ecosystem](https://github.com/sipcapture/homer) [![stars/year](https://img.shields.io/github/stars/sipcapture/homer?style=flat&color=gold&label=stars%2Fyear)](https://github.com/sipcapture/homer) [![commits/year](https://img.shields.io/github/commit-activity/y/sipcapture/homer?style=flat&color=blue&label=commits%2Fyear)](https://github.com/sipcapture/homer): open-source
  passive SIP/RTC capture interoperability and ladder/reporting model.
- [sngrep](https://github.com/irontec/sngrep) [![stars/year](https://img.shields.io/github/stars/irontec/sngrep?style=flat&color=gold&label=stars%2Fyear)](https://github.com/irontec/sngrep) [![commits/year](https://img.shields.io/github/commit-activity/y/irontec/sngrep?style=flat&color=blue&label=commits%2Fyear)](https://github.com/irontec/sngrep): open-source SIP ladder
  troubleshooting reference.
- [sipgrep](https://github.com/sipcapture/sipgrep) [![stars/year](https://img.shields.io/github/stars/sipcapture/sipgrep?style=flat&color=gold&label=stars%2Fyear)](https://github.com/sipcapture/sipgrep) [![commits/year](https://img.shields.io/github/commit-activity/y/sipcapture/sipgrep?style=flat&color=blue&label=commits%2Fyear)](https://github.com/sipcapture/sipgrep): open-source SIP packet
  sniffing and console exploration tool.
- [rtpbreak / rtpsplit](https://github.com/Naishy/rtpsplit) [![stars/year](https://img.shields.io/github/stars/Naishy/rtpsplit?style=flat&color=gold&label=stars%2Fyear)](https://github.com/Naishy/rtpsplit) [![commits/year](https://img.shields.io/github/commit-activity/y/Naishy/rtpsplit?style=flat&color=blue&label=commits%2Fyear)](https://github.com/Naishy/rtpsplit): open-source RTP
  reconstruction and analysis reference.
- [WebRTC Troubleshooter](https://github.com/webrtc/testrtc) [![stars/year](https://img.shields.io/github/stars/webrtc/testrtc?style=flat&color=gold&label=stars%2Fyear)](https://github.com/webrtc/testrtc) [![commits/year](https://img.shields.io/github/commit-activity/y/webrtc/testrtc?style=flat&color=blue&label=commits%2Fyear)](https://github.com/webrtc/testrtc): open-source
  client-side WebRTC diagnostics reference.
- [Trickle ICE sample](https://github.com/webrtc/samples/tree/gh-pages/src/content/peerconnection/trickle-ice) [![stars/year](https://img.shields.io/github/stars/webrtc/samples?style=flat&color=gold&label=stars%2Fyear)](https://github.com/webrtc/samples/tree/gh-pages/src/content/peerconnection/trickle-ice) [![commits/year](https://img.shields.io/github/commit-activity/y/webrtc/samples?style=flat&color=blue&label=commits%2Fyear)](https://github.com/webrtc/samples/tree/gh-pages/src/content/peerconnection/trickle-ice):
  open-source client-side ICE/NAT debug reference.
- [tcpdump](https://github.com/the-tcpdump-group/tcpdump) [![stars/year](https://img.shields.io/github/stars/the-tcpdump-group/tcpdump?style=flat&color=gold&label=stars%2Fyear)](https://github.com/the-tcpdump-group/tcpdump) [![commits/year](https://img.shields.io/github/commit-activity/y/the-tcpdump-group/tcpdump?style=flat&color=blue&label=commits%2Fyear)](https://github.com/the-tcpdump-group/tcpdump): open-source packet
  capture reference often used in RTC/VoIP investigations.
- [tshark / Wireshark](https://gitlab.com/wireshark/wireshark): open-source
  packet decode reference often used in RTC/VoIP investigations.

[Back to top](#awesome-rtc)

## WebRTC Servers, Gateways, And Media Apps

- [Janus Gateway](https://github.com/meetecho/janus-gateway) [![stars/year](https://img.shields.io/github/stars/meetecho/janus-gateway?style=flat&color=gold&label=stars%2Fyear)](https://github.com/meetecho/janus-gateway) [![commits/year](https://img.shields.io/github/commit-activity/y/meetecho/janus-gateway?style=flat&color=blue&label=commits%2Fyear)](https://github.com/meetecho/janus-gateway): open-source WebRTC
  gateway and media server.
- [LiveKit](https://github.com/livekit/livekit) [![stars/year](https://img.shields.io/github/stars/livekit/livekit?style=flat&color=gold&label=stars%2Fyear)](https://github.com/livekit/livekit) [![commits/year](https://img.shields.io/github/commit-activity/y/livekit/livekit?style=flat&color=blue&label=commits%2Fyear)](https://github.com/livekit/livekit): open-source WebRTC SFU/media
  infrastructure.
- [mediasoup](https://github.com/versatica/mediasoup) [![stars/year](https://img.shields.io/github/stars/versatica/mediasoup?style=flat&color=gold&label=stars%2Fyear)](https://github.com/versatica/mediasoup) [![commits/year](https://img.shields.io/github/commit-activity/y/versatica/mediasoup?style=flat&color=blue&label=commits%2Fyear)](https://github.com/versatica/mediasoup): open-source WebRTC SFU
  and conferencing framework.
- [Jitsi Videobridge](https://github.com/jitsi/jitsi-videobridge) [![stars/year](https://img.shields.io/github/stars/jitsi/jitsi-videobridge?style=flat&color=gold&label=stars%2Fyear)](https://github.com/jitsi/jitsi-videobridge) [![commits/year](https://img.shields.io/github/commit-activity/y/jitsi/jitsi-videobridge?style=flat&color=blue&label=commits%2Fyear)](https://github.com/jitsi/jitsi-videobridge) /
  [Jitsi Meet](https://github.com/jitsi/jitsi-meet) [![stars/year](https://img.shields.io/github/stars/jitsi/jitsi-meet?style=flat&color=gold&label=stars%2Fyear)](https://github.com/jitsi/jitsi-meet) [![commits/year](https://img.shields.io/github/commit-activity/y/jitsi/jitsi-meet?style=flat&color=blue&label=commits%2Fyear)](https://github.com/jitsi/jitsi-meet): open-source WebRTC
  conferencing and SFU reference stack.
- [Kurento](https://github.com/Kurento/kurento) [![stars/year](https://img.shields.io/github/stars/Kurento/kurento?style=flat&color=gold&label=stars%2Fyear)](https://github.com/Kurento/kurento) [![commits/year](https://img.shields.io/github/commit-activity/y/Kurento/kurento?style=flat&color=blue&label=commits%2Fyear)](https://github.com/Kurento/kurento): open-source WebRTC media
  server with media processing and recording.
- [Galene](https://github.com/jech/galene) [![stars/year](https://img.shields.io/github/stars/jech/galene?style=flat&color=gold&label=stars%2Fyear)](https://github.com/jech/galene) [![commits/year](https://img.shields.io/github/commit-activity/y/jech/galene?style=flat&color=blue&label=commits%2Fyear)](https://github.com/jech/galene): open-source lightweight
  video-conference server.
- [OpenVidu](https://github.com/OpenVidu/openvidu) [![stars/year](https://img.shields.io/github/stars/OpenVidu/openvidu?style=flat&color=gold&label=stars%2Fyear)](https://github.com/OpenVidu/openvidu) [![commits/year](https://img.shields.io/github/commit-activity/y/OpenVidu/openvidu?style=flat&color=blue&label=commits%2Fyear)](https://github.com/OpenVidu/openvidu): open-source
  video-conference platform built on WebRTC.
- [BigBlueButton](https://github.com/bigbluebutton/bigbluebutton) [![stars/year](https://img.shields.io/github/stars/bigbluebutton/bigbluebutton?style=flat&color=gold&label=stars%2Fyear)](https://github.com/bigbluebutton/bigbluebutton) [![commits/year](https://img.shields.io/github/commit-activity/y/bigbluebutton/bigbluebutton?style=flat&color=blue&label=commits%2Fyear)](https://github.com/bigbluebutton/bigbluebutton): open-source
  web conferencing system.
- [MiroTalk P2P](https://github.com/miroslavpejic85/mirotalk) [![stars/year](https://img.shields.io/github/stars/miroslavpejic85/mirotalk?style=flat&color=gold&label=stars%2Fyear)](https://github.com/miroslavpejic85/mirotalk) [![commits/year](https://img.shields.io/github/commit-activity/y/miroslavpejic85/mirotalk?style=flat&color=blue&label=commits%2Fyear)](https://github.com/miroslavpejic85/mirotalk) /
  [MiroTalk SFU](https://github.com/miroslavpejic85/mirotalksfu) [![stars/year](https://img.shields.io/github/stars/miroslavpejic85/mirotalksfu?style=flat&color=gold&label=stars%2Fyear)](https://github.com/miroslavpejic85/mirotalksfu) [![commits/year](https://img.shields.io/github/commit-activity/y/miroslavpejic85/mirotalksfu?style=flat&color=blue&label=commits%2Fyear)](https://github.com/miroslavpejic85/mirotalksfu): open-source
  WebRTC meeting references.
- [Plug-N-Meet](https://github.com/mynaparrot/plugNmeet-server) [![stars/year](https://img.shields.io/github/stars/mynaparrot/plugNmeet-server?style=flat&color=gold&label=stars%2Fyear)](https://github.com/mynaparrot/plugNmeet-server) [![commits/year](https://img.shields.io/github/commit-activity/y/mynaparrot/plugNmeet-server?style=flat&color=blue&label=commits%2Fyear)](https://github.com/mynaparrot/plugNmeet-server): open-source
  conferencing system built around LiveKit.
- [Medooze Media Server](https://github.com/medooze/media-server-node) [![stars/year](https://img.shields.io/github/stars/medooze/media-server-node?style=flat&color=gold&label=stars%2Fyear)](https://github.com/medooze/media-server-node) [![commits/year](https://img.shields.io/github/commit-activity/y/medooze/media-server-node?style=flat&color=blue&label=commits%2Fyear)](https://github.com/medooze/media-server-node):
  open-source Node WebRTC media server.
- [Kraken](https://github.com/MixinNetwork/kraken) [![stars/year](https://img.shields.io/github/stars/MixinNetwork/kraken?style=flat&color=gold&label=stars%2Fyear)](https://github.com/MixinNetwork/kraken) [![commits/year](https://img.shields.io/github/commit-activity/y/MixinNetwork/kraken?style=flat&color=blue&label=commits%2Fyear)](https://github.com/MixinNetwork/kraken): open-source Go WebRTC SFU.
- [OvenMediaEngine](https://github.com/AirenSoft/OvenMediaEngine) [![stars/year](https://img.shields.io/github/stars/AirenSoft/OvenMediaEngine?style=flat&color=gold&label=stars%2Fyear)](https://github.com/AirenSoft/OvenMediaEngine) [![commits/year](https://img.shields.io/github/commit-activity/y/AirenSoft/OvenMediaEngine?style=flat&color=blue&label=commits%2Fyear)](https://github.com/AirenSoft/OvenMediaEngine) /
  [OvenPlayer](https://github.com/AirenSoft/OvenPlayer) [![stars/year](https://img.shields.io/github/stars/AirenSoft/OvenPlayer?style=flat&color=gold&label=stars%2Fyear)](https://github.com/AirenSoft/OvenPlayer) [![commits/year](https://img.shields.io/github/commit-activity/y/AirenSoft/OvenPlayer?style=flat&color=blue&label=commits%2Fyear)](https://github.com/AirenSoft/OvenPlayer): open-source
  low-latency media streaming reference.
- [selkies-gstreamer](https://github.com/selkies-project/selkies-gstreamer) [![stars/year](https://img.shields.io/github/stars/selkies-project/selkies-gstreamer?style=flat&color=gold&label=stars%2Fyear)](https://github.com/selkies-project/selkies-gstreamer) [![commits/year](https://img.shields.io/github/commit-activity/y/selkies-project/selkies-gstreamer?style=flat&color=blue&label=commits%2Fyear)](https://github.com/selkies-project/selkies-gstreamer):
  open-source low-latency Linux WebRTC and GStreamer remote desktop/media
  components.
- [Pipecat](https://github.com/pipecat-ai/pipecat) [![stars/year](https://img.shields.io/github/stars/pipecat-ai/pipecat?style=flat&color=gold&label=stars%2Fyear)](https://github.com/pipecat-ai/pipecat) [![commits/year](https://img.shields.io/github/commit-activity/y/pipecat-ai/pipecat?style=flat&color=blue&label=commits%2Fyear)](https://github.com/pipecat-ai/pipecat): open-source voice/media
  pipeline reference.
- [VoiceBlender](https://github.com/voiceblender/voiceblender) [![stars/year](https://img.shields.io/github/stars/voiceblender/voiceblender?style=flat&color=gold&label=stars%2Fyear)](https://github.com/voiceblender/voiceblender) [![commits/year](https://img.shields.io/github/commit-activity/y/voiceblender/voiceblender?style=flat&color=blue&label=commits%2Fyear)](https://github.com/voiceblender/voiceblender): open-source
  SIP/WebRTC/AI voice service idea source.
- [Gossipper WebRTC](https://github.com/sipcapture/gossipper) [![stars/year](https://img.shields.io/github/stars/sipcapture/gossipper?style=flat&color=gold&label=stars%2Fyear)](https://github.com/sipcapture/gossipper) [![commits/year](https://img.shields.io/github/commit-activity/y/sipcapture/gossipper?style=flat&color=blue&label=commits%2Fyear)](https://github.com/sipcapture/gossipper): open-source
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
