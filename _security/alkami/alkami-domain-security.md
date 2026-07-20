---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: alkami.com
  spf: true
hosts:
- cert_expires: Oct  8 00:45:49 2026 GMT
  host: www.alkami.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Alkami Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Alkami, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Alkami
provider_slug: alkami
slug: alkami-domain-security
source_filename: alkami-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.alkami.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 00:45:49 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: alkami.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alkami/refs/heads/main/security/alkami-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Fintech
- Digital Banking
- Banking
- Credit Unions
- Financial Services
- Open Banking
- APIs
- SDK
---
