---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: sankun.com
  spf: true
hosts:
- cert_expires: Dec  2 23:59:59 2026 GMT
  host: sankun.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 10 21:00:22 2026 GMT
  host: data.sankun.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sankun Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sankun, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Sankun
provider_slug: sankun
slug: sankun-domain-security
source_filename: sankun-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sankun.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  2 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: data.sankun.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 21:00:22 2026 GMT\n  hsts: false\ndomains:\n- domain: sankun.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sankun/refs/heads/main/security/sankun-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Construction
- Big Data
- Data
- Real Estate
- Analytics
- CRM
- South Korea
---
