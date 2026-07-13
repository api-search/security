---
api_specs:
- filename: albertsons-retail-media-api-openapi.yml
  format: yaml
  label: Albertsons Media Collective API
  slug: retail-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/albertsons/refs/heads/main/openapi/albertsons-retail-media-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: albertsons.com
  spf: true
hosts:
- cert_expires: Sep  9 22:57:06 2026 GMT
  host: www.albertsons.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: portal-prod.apim.azwestus.stratus.albertsons.com
  https: false
- host: api.albertsons.com
  https: false
kind: domain-security
layout: security
method: probed
name: Albertsons Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for albertsons, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: albertsons
provider_slug: albertsons
slug: albertsons-domain-security
source_filename: albertsons-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.albertsons.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 22:57:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: portal-prod.apim.azwestus.stratus.albertsons.com\n  https: false\n- host: api.albertsons.com\n  https: false\ndomains:\n- domain: albertsons.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/albertsons/refs/heads/main/security/albertsons-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Grocery
- Retail
- Retail Media
- Advertising
- Campaigns
- Analytics
- Consumer Goods
- Food
- Pharmacy
---
