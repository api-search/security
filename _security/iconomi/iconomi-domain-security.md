---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: iconomi.com
  spf: true
hosts:
- cert_expires: Dec 10 01:26:17 2026 GMT
  host: iconomi.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Iconomi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ICONOMI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ICONOMI
provider_slug: iconomi
slug: iconomi-domain-security
source_filename: iconomi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: iconomi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 01:26:17 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: iconomi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/iconomi/security/iconomi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Crypto
- Asset Management
- Investment
- Platform
- Financial Services
- Company
---
