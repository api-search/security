---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: docdiffai.com
  spf: true
hosts:
- cert_expires: Jan 31 02:37:26 2027 GMT
  host: docdiffai.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Docdiffai Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DocDiffAI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: DocDiffAI
provider_slug: docdiffai-com
slug: docdiffai-com-domain-security
source_filename: docdiffai-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docdiffai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 31 02:37:26 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: docdiffai.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/docdiffai-com/security/docdiffai-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Document-Comparison
- Artificial Intelligence
- Software-as-a-Service
- Legal Tech
- Contract Management
- Company
---
