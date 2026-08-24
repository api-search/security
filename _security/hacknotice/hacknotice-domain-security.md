---
api_specs:
- filename: hacknotice-openapi.yml
  format: yaml
  label: HackNotice API
  slug: hacknotice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hacknotice/refs/heads/main/openapi/hacknotice-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: hacknotice.com
  spf: true
hosts:
- cert_expires: Oct 12 22:11:35 2026 GMT
  host: hacknotice.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 12 22:11:35 2026 GMT
  host: api-docs.hacknotice.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 14 23:59:59 2026 GMT
  host: extensionapi.hacknotice.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Hacknotice Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HackNotice, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: HackNotice
provider_slug: hacknotice
slug: hacknotice-domain-security
source_filename: hacknotice-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hacknotice.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 22:11:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api-docs.hacknotice.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 22:11:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: extensionapi.hacknotice.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 14 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: hacknotice.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hacknotice/refs/heads/main/security/hacknotice-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Security
- Threat Intelligence
- Cybersecurity
- Dark Web Monitoring
- Data Breaches
- Credential Monitoring
- Third Party Risk
- Vendor Risk Management
- Vulnerability Management
- Ransomware
- Security Assessments
- Alerts
- Monitoring
---
