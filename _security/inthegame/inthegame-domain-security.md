---
api_specs:
- filename: inthegame-openapi.yml
  format: yaml
  label: Inthegame API
  slug: inthegame-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inthegame/refs/heads/main/openapi/inthegame-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: inthegame.io
  spf: true
hosts:
- cert_expires: Sep 10 08:02:41 2026 GMT
  host: inthegame.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: api-dev.inthegame.io
  https: false
kind: domain-security
layout: security
method: probed
name: Inthegame Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Inthegame, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Inthegame
provider_slug: inthegame
slug: inthegame-domain-security
source_filename: inthegame-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: inthegame.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 08:02:41 2026 GMT\n  hsts: false\n- host: api-dev.inthegame.io\n  https: false\ndomains:\n- domain: inthegame.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/inthegame/refs/heads/main/security/inthegame-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Streaming
- CTV
- OTT
- Video
- Engagement
- Interactive
- Gamification
- Sports
- Real-time
---
