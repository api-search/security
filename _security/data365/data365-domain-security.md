---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: data365.co
  spf: false
hosts:
- cert_expires: Dec 13 10:13:48 2026 GMT
  host: data365.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Data365 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Data365, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Data365
provider_slug: data365
slug: data365-domain-security
source_filename: data365-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: data365.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 10:13:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: data365.co\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/data365/security/data365-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Social Media
- Real-Time Data
- Developers
---
