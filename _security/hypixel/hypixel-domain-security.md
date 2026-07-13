---
api_specs:
- filename: hypixel-public-api-openapi.yml
  format: yaml
  label: Hypixel Public API
  slug: hypixel-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hypixel/refs/heads/main/openapi/hypixel-public-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: hypixel.net
  spf: true
hosts:
- cert_expires: Sep  8 19:07:04 2026 GMT
  host: hypixel.net
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  8 19:07:04 2026 GMT
  host: api.hypixel.net
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hypixel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hypixel, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Hypixel
provider_slug: hypixel
slug: hypixel-domain-security
source_filename: hypixel-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hypixel.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 19:07:04 2026 GMT\n  hsts: null\n- host: api.hypixel.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 19:07:04 2026 GMT\n  hsts: false\ndomains:\n- domain: hypixel.net\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hypixel/refs/heads/main/security/hypixel-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Games And Comics
- Gaming
- Minecraft
- Player Stats
- Leaderboards
- SkyBlock
- Public APIs
---
