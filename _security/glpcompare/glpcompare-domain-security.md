---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: glpcompare.co
  spf: false
hosts:
- cert_expires: Jan  8 16:01:49 2027 GMT
  host: glpcompare.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: GLPcompare Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GLPcompare, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: GLPcompare
provider_slug: glpcompare
slug: glpcompare-domain-security
source_filename: glpcompare-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: glpcompare.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 16:01:49 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: glpcompare.co\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/glpcompare/security/glpcompare-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- GLP-1
- Pricing
- Healthcare
- Free
---
