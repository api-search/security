---
api_specs:
- filename: pinnacle-openapi.yml
  format: yaml
  label: Pinnacle Customer API
  slug: pinnacle-customer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinnacle-sports-betting/refs/heads/main/openapi/pinnacle-openapi.yml
- filename: pinnacle-asyncapi.yml
  format: yaml
  label: Pinnacle Lines API
  slug: pinnacle-lines-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinnacle-sports-betting/refs/heads/main/openapi/pinnacle-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: pinnacle.com
  spf: true
hosts:
- cert_expires: Sep 22 17:18:28 2026 GMT
  host: www.pinnacle.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 17:18:28 2026 GMT
  host: api.pinnacle.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pinnacle Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for  Pinnacle Sports Betting, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ' Pinnacle Sports Betting'
provider_slug: pinnacle-sports-betting
slug: pinnacle-domain-security
source_filename: pinnacle-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.pinnacle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 17:18:28 2026 GMT\n  hsts: true\n  hsts_max_age: 0\n- host: api.pinnacle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 17:18:28 2026 GMT\n  hsts: null\ndomains:\n- domain: pinnacle.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pinnacle-sports-betting/refs/heads/main/security/pinnacle-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Gambling
- Sports Betting
---
