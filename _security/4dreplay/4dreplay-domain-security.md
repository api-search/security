---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: 4dreplay.com
  spf: true
- caa: []
  dmarc: false
  dmarc_policy: null
  dnssec: false
  domain: 4dist.com
  spf: false
hosts:
- cert_expires: Oct 21 23:22:32 2026 GMT
  host: 4dreplay.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 15 15:37:16 2026 GMT
  host: 4dist.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: 4Dreplay Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 4DReplay, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: 4DReplay
provider_slug: 4dreplay
slug: 4dreplay-domain-security
source_filename: 4dreplay-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 4dreplay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 23:22:32 2026 GMT\n  hsts: false\n- host: 4dist.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 15:37:16 2026 GMT\n  hsts: false\ndomains:\n- domain: 4dreplay.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: 4dist.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n  dmarc_policy: null\nfindings:\n- No HSTS on either host.\n- No CAA records on either registrable domain.\n- No DNSSEC on either registrable domain.\n- 4dist.com publishes neither SPF nor DMARC; 4dreplay.com publishes both, but DMARC policy is p=none (monitor only).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/4dreplay/refs/heads/main/security/4dreplay-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Video
- Sports
- Media
- Broadcasting
- Streaming
- OTT
- Artificial Intelligence
- Computer Vision
- Entertainment
---
