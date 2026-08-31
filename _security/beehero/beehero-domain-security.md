---
api_specs:
- filename: beehero-audio-api-openapi.yml
  format: yaml
  label: BeeHero Audio API
  slug: beehero-audio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beehero/refs/heads/main/openapi/beehero-audio-api-openapi.yml
- filename: beehero-auth-api-openapi.yml
  format: yaml
  label: BeeHero Auth API
  slug: beehero-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beehero/refs/heads/main/openapi/beehero-auth-api-openapi.yml
- filename: beehero-gateways-api-openapi.yml
  format: yaml
  label: BeeHero Gateways API
  slug: beehero-gateways-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beehero/refs/heads/main/openapi/beehero-gateways-api-openapi.yml
- filename: beehero-sensors-api-openapi.yml
  format: yaml
  label: BeeHero Sensors API
  slug: beehero-sensors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beehero/refs/heads/main/openapi/beehero-sensors-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: beehero.io
  spf: true
hosts:
- cert_expires: Oct 14 17:49:31 2026 GMT
  host: www.beehero.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  5 23:59:59 2026 GMT
  host: docs.beehero.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 27 23:59:59 2026 GMT
  host: backend.beehero.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Beehero Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BeeHero, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: BeeHero
provider_slug: beehero
slug: beehero-domain-security
source_filename: beehero-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.beehero.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 17:49:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.beehero.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  5 23:59:59 2026 GMT\n  hsts: false\n- host: backend.beehero.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: beehero.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/beehero/refs/heads/main/security/beehero-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Agriculture
- agtech
- pollination
- beekeeping
- precision-agriculture
- iot
- sensors
- environmental-data
- MCP
- agent-native
---
