---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: celum.com
  spf: true
hosts:
- cert_expires: Feb  4 04:53:01 2027 GMT
  host: celum.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: CELUM Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CELUM, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: CELUM
provider_slug: celum
slug: celum-domain-security
source_filename: celum-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: celum.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  4 04:53:01 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: celum.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/celum/security/celum-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Digital Asset Management
- Content Management
- Artificial Intelligence
- Enterprise
---
