---
api_specs:
- filename: gamerpower-filter-api-openapi.yml
  format: yaml
  label: GamerPower Filter API
  slug: gamerpower-filter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gamerpower/refs/heads/main/openapi/gamerpower-filter-api-openapi.yml
- filename: gamerpower-giveaways-api-openapi.yml
  format: yaml
  label: GamerPower Giveaways API
  slug: gamerpower-giveaways-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gamerpower/refs/heads/main/openapi/gamerpower-giveaways-api-openapi.yml
- filename: gamerpower-worth-api-openapi.yml
  format: yaml
  label: GamerPower Worth API
  slug: gamerpower-worth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gamerpower/refs/heads/main/openapi/gamerpower-worth-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: gamerpower.com
  spf: true
hosts:
- cert_expires: Aug 30 14:48:05 2026 GMT
  host: www.gamerpower.com
  hsts: true
  hsts_max_age: 16070400
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gamerpower Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GamerPower, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: GamerPower
provider_slug: gamerpower
slug: gamerpower-domain-security
source_filename: gamerpower-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gamerpower.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 14:48:05 2026 GMT\n  hsts: true\n  hsts_max_age: 16070400\ndomains:\n- domain: gamerpower.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gamerpower/refs/heads/main/security/gamerpower-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Games And Comics
- Giveaways
- Free Games
- Public APIs
---
