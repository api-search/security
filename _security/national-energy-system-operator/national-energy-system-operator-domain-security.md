---
api_specs:
- filename: national-energy-system-operator-openapi.json
  format: json
  label: NESO Data Portal API
  slug: data-portal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/national-energy-system-operator/main/openapi/national-energy-system-operator-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: neso.energy
  spf: true
hosts:
- cert_expires: Aug 30 15:27:23 2026 GMT
  host: www.neso.energy
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  2 17:07:34 2026 GMT
  host: api.neso.energy
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: National Energy System Operator Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for National Energy System Operator, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: National Energy System Operator
provider_slug: national-energy-system-operator
slug: national-energy-system-operator-domain-security
source_filename: national-energy-system-operator-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.neso.energy\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 15:27:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.neso.energy\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 17:07:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: neso.energy\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/national-energy-system-operator/refs/heads/main/security/national-energy-system-operator-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Energy
- Electricity
- Grid
- Open Data
- United Kingdom
---
