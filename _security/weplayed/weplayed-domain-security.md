---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: weplayed.com
  spf: true
hosts:
- cert_expires: Mar  7 23:59:59 2027 GMT
  host: weplayed.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Weplayed Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for WePlayed, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: WePlayed
provider_slug: weplayed
slug: weplayed-domain-security
source_filename: weplayed-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: weplayed.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  7 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: weplayed.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/weplayed/refs/heads/main/security/weplayed-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Sports
- Video
- Artificial Intelligence
- Media
- College Athletics
- Highlights
- Short-Form Video
---
