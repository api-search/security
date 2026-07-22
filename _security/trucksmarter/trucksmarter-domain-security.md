---
api_specs:
- filename: trucksmarter-load-posting-openapi.yml
  format: yaml
  label: TruckSmarter Load Posting API
  slug: trucksmarter-load-posting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trucksmarter/refs/heads/main/openapi/trucksmarter-load-posting-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: trucksmarter.com
  spf: true
hosts:
- cert_expires: Oct 11 21:13:14 2026 GMT
  host: www.trucksmarter.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 16 23:59:59 2027 GMT
  host: api.trucksmarter.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Trucksmarter Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TruckSmarter, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: TruckSmarter
provider_slug: trucksmarter
slug: trucksmarter-domain-security
source_filename: trucksmarter-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.trucksmarter.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 21:13:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.trucksmarter.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 16 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: trucksmarter.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trucksmarter/refs/heads/main/security/trucksmarter-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Trucking
- Freight
- Logistics
- Load Board
- Transportation
- Dispatch
- Fuel
- Factoring
---
