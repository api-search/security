---
api_specs:
- filename: department-of-energy-openapi.yml
  format: yaml
  label: EIA Open Data API V2
  slug: eia-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-energy/refs/heads/main/openapi/department-of-energy-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: energy.gov
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: eia.gov
  spf: true
hosts:
- cert_expires: Sep 26 23:59:59 2026 GMT
  host: www.energy.gov
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 19 23:59:59 2026 GMT
  host: www.eia.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 17:20:52 2026 GMT
  host: api.eia.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Department Of Energy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Department of Energy, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Department of Energy
provider_slug: department-of-energy
slug: department-of-energy-domain-security
source_filename: department-of-energy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.energy.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.eia.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 23:59:59 2026 GMT\n  hsts: null\n- host: api.eia.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 17:20:52 2026 GMT\n  hsts: null\ndomains:\n- domain: energy.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: eia.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/department-of-energy/refs/heads/main/security/department-of-energy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Buildings
- Electricity
- Energy
- Federal Government
- Open Data
- Renewables
- Research
- Solar
- Statistics
---
