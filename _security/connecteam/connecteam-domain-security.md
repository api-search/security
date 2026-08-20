---
api_specs:
- filename: connecteam-openapi-original.json
  format: json
  label: Connecteam API
  slug: api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/connecteam/refs/heads/main/openapi/connecteam-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: connecteam.com
  spf: true
hosts:
- cert_expires: Oct  5 15:25:35 2026 GMT
  host: connecteam.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 04:36:52 2026 GMT
  host: developer.connecteam.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 15:25:35 2026 GMT
  host: api.connecteam.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Connecteam Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Connecteam, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Connecteam
provider_slug: connecteam
slug: connecteam-domain-security
source_filename: connecteam-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: connecteam.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 15:25:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.connecteam.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 04:36:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.connecteam.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 15:25:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: connecteam.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/connecteam/refs/heads/main/security/connecteam-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Workforce Management
- Human Resources
- Time Tracking
- Scheduling
- Employee Communication
- Task Management
- Forms
- Deskless
- Software-as-a-Service
---
