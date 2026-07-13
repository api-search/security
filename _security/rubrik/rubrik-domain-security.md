---
api_specs:
- filename: rubrik-openapi.yml
  format: yaml
  label: Rubrik Security Cloud API
  slug: rubrik-security-cloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rubrik/refs/heads/main/openapi/rubrik-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: rubrik.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: terraform.io
  spf: true
hosts:
- cert_expires: Jan  5 23:59:59 2027 GMT
  host: www.rubrik.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 08:13:48 2026 GMT
  host: developer.rubrik.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 19 23:59:59 2026 GMT
  host: registry.terraform.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rubrik Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rubrik, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Rubrik
provider_slug: rubrik
slug: rubrik-domain-security
source_filename: rubrik-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rubrik.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 23:59:59 2027 GMT\n  hsts: null\n- host: developer.rubrik.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 08:13:48 2026 GMT\n  hsts: false\n- host: registry.terraform.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 19 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: rubrik.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: terraform.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rubrik/refs/heads/main/security/rubrik-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Backup
- Cyber Recovery
- Data Security
- Data Security Posture Management
- GraphQL
- Ransomware Recovery
- REST API
- SaaS Protection
- Threat Analytics
- Zero Trust
---
