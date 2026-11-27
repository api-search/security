---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: arison8.com
  spf: true
hosts:
- cert_expires: Dec  9 22:25:31 2026 GMT
  host: arison8.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: ARISON8 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ARISON8, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ARISON8
provider_slug: arison8-com
slug: arison8-com-domain-security
source_filename: arison8-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: arison8.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 22:25:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: arison8.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/arison8-com/security/arison8-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Software-as-a-Service
- Software
- Florida
- Mobile
---
