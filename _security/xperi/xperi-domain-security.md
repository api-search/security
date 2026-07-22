---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: xperi.com
  spf: true
hosts:
- cert_expires: Oct  5 18:04:19 2026 GMT
  host: xperi.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Xperi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Xperi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Xperi
provider_slug: xperi
slug: xperi-domain-security
source_filename: xperi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: xperi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 18:04:19 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: xperi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xperi/refs/heads/main/security/xperi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Entertainment
- Media
- Audio
- Connected Car
- Consumer Electronics
- Streaming
- Television
- Digital Radio
---
