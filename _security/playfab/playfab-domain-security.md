---
api_specs:
- filename: playfab-openapi.yml
  format: yaml
  label: PlayFab Client API
  slug: playfab-client-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/playfab/refs/heads/main/openapi/playfab-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "microsoft.com"
  - 128 contactemail "caarecordaware@microsoft.com"
  - 0 iodef "mailto:caarecordaware@microsoft.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: playfab.com
  spf: true
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: microsoft.com
  spf: true
hosts:
- cert_expires: Jan 23 23:59:59 2027 GMT
  host: playfab.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  4 05:56:36 2026 GMT
  host: developer.playfab.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 11 02:26:09 2026 GMT
  host: learn.microsoft.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Playfab Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PlayFab, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: PlayFab
provider_slug: playfab
slug: playfab-domain-security
source_filename: playfab-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: playfab.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.playfab.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 05:56:36 2026 GMT\n  hsts: null\n- host: learn.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 02:26:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: playfab.com\n  dnssec: false\n  caa:\n  - 0 issue \"microsoft.com\"\n  - 128 contactemail \"caarecordaware@microsoft.com\"\n  - 0 iodef \"mailto:caarecordaware@microsoft.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: microsoft.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/playfab/refs/heads/main/security/playfab-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Authentication
- Azure
- Backend
- BaaS
- CloudScript
- Economy
- Game Backend
- Game Development
- Games
- Leaderboards
- Matchmaking
- Microsoft
- Multiplayer
- PlayFab
- REST
---
