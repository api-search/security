---
api_specs:
- filename: bored-api-openapi.yml
  format: yaml
  label: Bored API
  slug: bored-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bored-api/refs/heads/main/openapi/bored-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: appbrewery.com
  spf: true
hosts:
- cert_expires: Aug 21 02:59:42 2026 GMT
  host: bored-api.appbrewery.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bored Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bored API, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Bored API
provider_slug: bored-api
slug: bored-api-domain-security
source_filename: bored-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bored-api.appbrewery.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 02:59:42 2026 GMT\n  hsts: false\ndomains:\n- domain: appbrewery.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bored-api/refs/heads/main/security/bored-api-domain-security.yml
summary_line: TLSv1.3
tags:
- Activities
- Boredom
- Random
- Entertainment
- Lifestyle
- Free
---
