---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: lomenanalytics.com
  spf: true
hosts:
- cert_expires: Feb  1 14:55:33 2027 GMT
  host: lomenanalytics.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Lomen Analytics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lomen Analytics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Lomen Analytics
provider_slug: lomenanalytics-com
slug: lomenanalytics-com-domain-security
source_filename: lomenanalytics-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lomenanalytics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  1 14:55:33 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: lomenanalytics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/lomenanalytics-com/security/lomenanalytics-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Analytics
- Privacy
- Artificial Intelligence
- Websites
- Cookie-Free
---
