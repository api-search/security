---
api_specs:
- filename: entergy-wordpress-rest-openapi.yml
  format: yaml
  label: Entergy WordPress REST API
  slug: entergy-wordpress-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/entergy/refs/heads/main/openapi/entergy-wordpress-rest-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: entergy.com
  spf: true
hosts:
- cert_expires: Nov 13 16:18:48 2026 GMT
  host: www.entergy.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Entergy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Entergy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Entergy
provider_slug: entergy
slug: entergy-domain-security
source_filename: entergy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.entergy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 13 16:18:48 2026 GMT\n  hsts: null\ndomains:\n- domain: entergy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/entergy/refs/heads/main/security/entergy-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Electricity
- Energy
- Fortune 500
- Utility
- Nuclear
- Power Generation
- Louisiana
- Geospatial
---
