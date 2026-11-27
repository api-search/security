---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: opula.io
  spf: true
hosts:
- cert_expires: Jan 25 07:05:46 2027 GMT
  host: opula.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Opula Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Opula, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Opula
provider_slug: opula-io
slug: opula-io-domain-security
source_filename: opula-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: opula.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 25 07:05:46 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: opula.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/opula-io/security/opula-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Finance
- Personal Finance
- Artificial Intelligence
- Investment
- Analytics
- Company
---
