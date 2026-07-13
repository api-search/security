---
api_specs:
- filename: vehicle-databases-openapi.yml
  format: yaml
  label: Vehicle Databases Maintenance API
  slug: vehicle-databases
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vehicle-databases/refs/heads/main/openapi/vehicle-databases-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: vehicledatabases.com
  spf: true
hosts:
- cert_expires: Sep 12 11:35:42 2026 GMT
  host: vehicledatabases.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 07:24:49 2026 GMT
  host: api.vehicledatabases.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vehicle Databases Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vehicle Databases, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Vehicle Databases
provider_slug: vehicle-databases
slug: vehicle-databases-domain-security
source_filename: vehicle-databases-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vehicledatabases.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 11:35:42 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.vehicledatabases.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 07:24:49 2026 GMT\n  hsts: null\ndomains:\n- domain: vehicledatabases.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vehicle-databases/refs/heads/main/security/vehicle-databases-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Automotive
- Fleet Management
- Maintenance
- Recalls
- Vehicles
---
