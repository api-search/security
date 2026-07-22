---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: voya.com
  spf: true
hosts:
- cert_expires: Aug  5 03:13:08 2026 GMT
  host: www.voya.com
  hsts: true
  hsts_max_age: 31622400
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Voya Financial Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Voya Financial, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Voya Financial
provider_slug: voya-financial
slug: voya-financial-domain-security
source_filename: voya-financial-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.voya.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug  5 03:13:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31622400\ndomains:\n- domain: voya.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/voya-financial/refs/heads/main/security/voya-financial-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC · DMARC
tags:
- Benefits
- Finance
- Fortune 500
- Health Savings
- Investment Management
- Retirement
---
