---
api_specs:
- filename: openapi.json
  format: json
  label: Itch.io API
  slug: itch-io-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/itch-io/refs/heads/main/openapi/openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: itch.io
  spf: true
hosts:
- cert_expires: Sep 20 13:15:02 2026 GMT
  host: itch.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 13:15:02 2026 GMT
  host: api.itch.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Itch Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Itch.io, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Itch.io
provider_slug: itch-io
slug: itch-io-domain-security
source_filename: itch-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: itch.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 13:15:02 2026 GMT\n  hsts: false\n- host: api.itch.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 13:15:02 2026 GMT\n  hsts: null\ndomains:\n- domain: itch.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/itch-io/refs/heads/main/security/itch-io-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Games
- Indie Games
- Game Distribution
- Game Marketplace
- Developers
---
