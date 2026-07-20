---
api_specs:
- filename: flipturn-openapi.yml
  format: yaml
  label: Flipturn API
  slug: flipturn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flipturn/refs/heads/main/openapi/flipturn-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: getflipturn.com
  spf: true
hosts:
- cert_expires: Sep 12 11:57:08 2026 GMT
  host: www.getflipturn.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 00:49:43 2026 GMT
  host: api.getflipturn.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Flipturn Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Flipturn, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Flipturn
provider_slug: flipturn
slug: flipturn-domain-security
source_filename: flipturn-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.getflipturn.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 11:57:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.getflipturn.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 00:49:43 2026 GMT\n  hsts: null\ndomains:\n- domain: getflipturn.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flipturn/refs/heads/main/security/flipturn-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- EV Charging
- Electric Vehicles
- Fleet Management
- Energy
- Charging Infrastructure
- OCPP
- OCPI
- Mobility
- REST API
---
