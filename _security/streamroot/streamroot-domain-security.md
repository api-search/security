---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: streamroot.io
  spf: false
hosts:
- host: streamroot.io
  https: false
kind: domain-security
layout: security
method: probed
name: Streamroot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Streamroot, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Streamroot
provider_slug: streamroot
slug: streamroot-domain-security
source_filename: streamroot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: streamroot.io\n  https: false\ndomains:\n- domain: streamroot.io\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/streamroot/refs/heads/main/security/streamroot-domain-security.yml
summary_line: DNSSEC
tags:
- Company
- Infrastructure Saas
- Video
- Streaming
- CDN
- Peer To Peer
- WebRTC
- Media Delivery
- SDK
- Acquired
---
