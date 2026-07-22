---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: aicepower.com
  spf: true
hosts:
- cert_expires: Sep 27 19:22:58 2026 GMT
  host: aicepower.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aice Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AICE, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: AICE
provider_slug: aice
slug: aice-domain-security
source_filename: aice-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aicepower.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 19:22:58 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: aicepower.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aice/refs/heads/main/security/aice-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Defense
- Robotics
- Autonomous Systems
- Maritime
- Underwater Drones
- Hardware
- Y Combinator
---
