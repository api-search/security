---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: gamestop.com
  spf: true
hosts:
- cert_expires: Jan 29 23:07:20 2027 GMT
  host: www.gamestop.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gamestop Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GameStop, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: GameStop
provider_slug: gamestop
slug: gamestop-domain-security
source_filename: gamestop-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gamestop.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 29 23:07:20 2027 GMT\n  hsts: null\ndomains:\n- domain: gamestop.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gamestop/refs/heads/main/security/gamestop-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Consumer Electronics
- Gaming
- Retail
- Fortune 500
---
