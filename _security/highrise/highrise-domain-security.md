---
api_specs:
- filename: highrise-bot-api-asyncapi.yml
  format: yaml
  label: Highrise Bot API
  slug: highrise-bot-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/highrise/refs/heads/main/asyncapi/highrise-bot-api-asyncapi.yml
- filename: highrise-web-api-openapi.yml
  format: yaml
  label: Highrise Web API
  slug: highrise-web-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/highrise/refs/heads/main/openapi/highrise-web-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: highrise.game
  spf: false
hosts:
- cert_expires: Sep 13 08:30:50 2026 GMT
  host: highrise.game
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 08:30:50 2026 GMT
  host: create.highrise.game
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 08:30:50 2026 GMT
  host: webapi.highrise.game
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Highrise Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Highrise, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Highrise
provider_slug: highrise
slug: highrise-domain-security
source_filename: highrise-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: highrise.game\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 08:30:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: create.highrise.game\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 08:30:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: webapi.highrise.game\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 08:30:50 2026 GMT\n  hsts: null\ndomains:\n- domain: highrise.game\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/highrise/refs/heads/main/security/highrise-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Virtual World
- Metaverse
- Social
- Gaming
- Avatars
- Bots
- Developer Platform
- Chat
---
