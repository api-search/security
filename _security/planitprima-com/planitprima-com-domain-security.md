---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: planitprima.com
  spf: true
hosts:
- cert_expires: Jan 16 23:59:59 2027 GMT
  host: planitprima.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Planitprima Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for planitprima-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: planitprima-com
provider_slug: planitprima-com
slug: planitprima-com-domain-security
source_filename: planitprima-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: planitprima.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: planitprima.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/planitprima-com/security/planitprima-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Data-Protection
- GDPR
- SaaS
- Privacy
- Compliance
- Software
---
