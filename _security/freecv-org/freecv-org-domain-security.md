---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: freecv.org
  spf: true
hosts:
- cert_expires: Feb  1 01:41:10 2027 GMT
  host: freecv.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: FreeCV Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FreeCV, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: FreeCV
provider_slug: freecv-org
slug: freecv-org-domain-security
source_filename: freecv-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: freecv.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  1 01:41:10 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: freecv.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/freecv-org/security/freecv-org-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Resume Builder
- Artificial Intelligence
- Free
- Job Search
---
