---
api_specs:
- filename: utilityapi-openapi.yml
  format: yaml
  label: UtilityAPI
  slug: utilityapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/utilityapi/refs/heads/main/openapi/utilityapi-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: utilityapi.com
  spf: true
hosts:
- cert_expires: Aug 17 19:11:25 2026 GMT
  host: utilityapi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Utilityapi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for UtilityAPI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: UtilityAPI
provider_slug: utilityapi
slug: utilityapi-domain-security
source_filename: utilityapi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: utilityapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 19:11:25 2026 GMT\n  hsts: false\ndomains:\n- domain: utilityapi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/utilityapi/refs/heads/main/security/utilityapi-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Energy
- Utilities
- Green Button
- Billing Data
- Meter Data
- Clean Energy
---
