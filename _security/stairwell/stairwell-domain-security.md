---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: stairwell.com
  spf: true
hosts:
- cert_expires: Sep  2 20:51:11 2026 GMT
  host: www.stairwell.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  3 05:42:50 2026 GMT
  host: docs.stairwell.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  9 03:14:13 2026 GMT
  host: app.stairwell.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Stairwell Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Stairwell, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Stairwell
provider_slug: stairwell
slug: stairwell-domain-security
source_filename: stairwell-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.stairwell.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 20:51:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.stairwell.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 05:42:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.stairwell.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 03:14:13 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: stairwell.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stairwell/refs/heads/main/security/stairwell-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Security
- Threat Intelligence
- Malware Analysis
- Cybersecurity
- Threat Detection
- YARA
- Incident Response
---
