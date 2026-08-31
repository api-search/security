---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: runbooks.com
  spf: true
hosts:
- cert_expires: Oct  4 07:43:28 2026 GMT
  host: runbooks.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Runbooks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Runbooks, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Runbooks
provider_slug: runbooks
slug: runbooks-domain-security
source_filename: runbooks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: runbooks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 07:43:28 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: runbooks.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/runbooks/refs/heads/main/security/runbooks-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- ITSM
- ITAM
- IT Operations
- Managed Service Provider
- Help Desk
- Asset Management
- Incident Management
- Security Operations
- CRM
- IT Service Management
---
