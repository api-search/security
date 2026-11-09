---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: burofacil.es
  spf: true
hosts:
- cert_expires: Dec 12 23:22:24 2026 GMT
  host: burofacil.es
  hsts: true
  hsts_max_age: 15724800
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Burofacil Es Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Burofácil, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Burofácil
provider_slug: burofacil-es
slug: burofacil-es-domain-security
source_filename: burofacil-es-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: burofacil.es\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 23:22:24 2026 GMT\n  hsts: true\n  hsts_max_age: 15724800\ndomains:\n- domain: burofacil.es\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/burofacil-es/security/burofacil-es-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Legal Tech
- Document Automation
- Spain
- Certified Mail
- Burofax
---
