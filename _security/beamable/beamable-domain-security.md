---
api_specs:
- filename: beamable-basic-api-openapi.yml
  format: yaml
  label: Beamable Basic API
  slug: beamable-basic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beamable/refs/heads/main/openapi/beamable-basic-api-openapi.yml
- filename: beamable-object-api-openapi.yml
  format: yaml
  label: Beamable Object API
  slug: beamable-object-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beamable/refs/heads/main/openapi/beamable-object-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: beamable.com
  spf: true
hosts:
- cert_expires: Aug 26 05:34:01 2026 GMT
  host: beamable.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  6 06:59:57 2026 GMT
  host: docs.beamable.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 16 23:59:59 2026 GMT
  host: api.beamable.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Beamable Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Beamable, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Beamable
provider_slug: beamable
slug: beamable-domain-security
source_filename: beamable-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: beamable.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 05:34:01 2026 GMT\n  hsts: false\n- host: docs.beamable.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 06:59:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.beamable.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 16 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: beamable.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/beamable/refs/heads/main/security/beamable-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Game Backend
- LiveOps
- Player Accounts
- Virtual Currency
- Inventory
- Leaderboards
- Matchmaking
- Microservices
- Unity
- Unreal
- Game Economy
- Analytics
---
