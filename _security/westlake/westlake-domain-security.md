---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: westlake.com
  spf: true
hosts:
- cert_expires: Aug  7 23:59:59 2026 GMT
  host: www.westlake.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Westlake Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Westlake, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Westlake
provider_slug: westlake
slug: westlake-domain-security
source_filename: westlake-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.westlake.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  7 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: westlake.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/westlake/refs/heads/main/security/westlake-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Chemicals
- Polymers
- Building Products
- Manufacturing
- Fortune 500
---
