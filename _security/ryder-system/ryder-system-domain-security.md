---
api_specs:
- filename: ryder-fleet-management-api-openapi.yml
  format: yaml
  label: Ryder Fleet Management API
  slug: fleet-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ryder-system/refs/heads/main/openapi/ryder-fleet-management-api-openapi.yml
- filename: ryder-carrier-api-openapi.yml
  format: yaml
  label: Ryder Carrier API
  slug: carrier-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ryder-system/refs/heads/main/openapi/ryder-carrier-api-openapi.yml
- filename: ryder-tm-shipment-api-openapi.yml
  format: yaml
  label: Ryder TM Shipment Management API
  slug: tm-shipment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ryder-system/refs/heads/main/openapi/ryder-tm-shipment-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ryder.com
  spf: true
hosts:
- cert_expires: Nov 20 23:59:59 2026 GMT
  host: www.ryder.com
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 23:59:59 2026 GMT
  host: developer.ryder.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 20 23:59:59 2026 GMT
  host: api.ryder.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ryder System Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ryder System, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Ryder System
provider_slug: ryder-system
slug: ryder-system-domain-security
source_filename: ryder-system-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ryder.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 86400\n- host: developer.ryder.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.ryder.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: ryder.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ryder-system/refs/heads/main/security/ryder-system-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fleet Management
- Logistics
- Supply Chain
- Transportation
- Trucking
- Fortune 500
---
