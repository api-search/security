---
api_specs:
- filename: empirical-security-openapi.yml
  format: yaml
  label: Empirical Security API
  slug: empirical-security-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/empirical-security/refs/heads/main/openapi/empirical-security-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: empiricalsecurity.com
  spf: true
hosts:
- cert_expires: Sep 23 23:49:15 2026 GMT
  host: www.empiricalsecurity.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  5 23:59:59 2027 GMT
  host: app.empiricalsecurity.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Empirical Security Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Empirical Security, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Empirical Security
provider_slug: empirical-security
slug: empirical-security-domain-security
source_filename: empirical-security-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.empiricalsecurity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 23:49:15 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: app.empiricalsecurity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  5 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: empiricalsecurity.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/empirical-security/refs/heads/main/security/empirical-security-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Security
- Cybersecurity
- Vulnerability Management
- Vulnerability Prioritization
- CVE
- EPSS
- Exploit Prediction
- Threat Intelligence
---
