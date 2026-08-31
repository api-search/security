---
api_specs:
- filename: llms.txt
  format: yaml
  label: Motive Fleet API
  slug: motive-fleet-api
  spec_type: OpenAPI
  url: https://developer-docs.gomotive.com/llms.txt
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: gomotive.com
  spf: true
hosts:
- cert_expires: Oct  7 03:21:57 2026 GMT
  host: gomotive.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 27 23:59:59 2026 GMT
  host: developer.gomotive.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Dec 29 23:59:59 2026 GMT
  host: api.gomotive.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Motive Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Motive, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Motive
provider_slug: motive
slug: motive-domain-security
source_filename: motive-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gomotive.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 03:21:57 2026 GMT\n  hsts: false\n- host: developer.gomotive.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 27 23:59:59 2026 GMT\n  hsts: false\n- host: api.gomotive.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 29 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: gomotive.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/motive/refs/heads/main/security/motive-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Fleet Management
- Trucking
- Logistics
- GPS Tracking
- Hours of Service
- ELD
- IFTA
- Dashcam
- Dispatch
- Compliance
- Driver Management
---
