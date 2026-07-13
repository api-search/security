---
api_specs:
- filename: tesla-openapi-original.yml
  format: yaml
  label: Tesla Fleet API
  slug: fleet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tesla/refs/heads/main/openapi/tesla-openapi-original.yml
- filename: tesla-openapi-original.yml
  format: yaml
  label: Tesla Owner API
  slug: owner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tesla/refs/heads/main/openapi/tesla-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tesla.com
  spf: true
hosts:
- cert_expires: Nov 17 23:59:59 2026 GMT
  host: developer.tesla.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 17 23:59:59 2026 GMT
  host: www.tesla.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 18 23:59:59 2026 GMT
  host: fleet-api.prd.na.vn.cloud.tesla.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tesla Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tesla, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Tesla
provider_slug: tesla
slug: tesla-domain-security
source_filename: tesla-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.tesla.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\n- host: www.tesla.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 23:59:59 2026 GMT\n  hsts: null\n- host: fleet-api.prd.na.vn.cloud.tesla.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: tesla.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tesla/refs/heads/main/security/tesla-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Automobiles
- Cars
- Vehicles
- Electric Vehicles
- Energy
- Clean Energy
- IoT
---
