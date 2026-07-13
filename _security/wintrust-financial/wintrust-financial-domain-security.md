---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: wintrust.com
  spf: true
hosts:
- cert_expires: Feb 13 23:59:59 2027 GMT
  host: www.wintrust.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
- host: developer.wintrust.com
  https: false
- host: api.wintrust.com
  https: false
kind: domain-security
layout: security
method: probed
name: Wintrust Financial Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wintrust Financial, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Wintrust Financial
provider_slug: wintrust-financial
slug: wintrust-financial-domain-security
source_filename: wintrust-financial-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.wintrust.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 13 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: developer.wintrust.com\n  https: false\n- host: api.wintrust.com\n  https: false\ndomains:\n- domain: wintrust.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wintrust-financial/refs/heads/main/security/wintrust-financial-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Banking
- Financial Services
- Community
---
