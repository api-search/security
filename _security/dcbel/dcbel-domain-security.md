---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: dcbel.energy
  spf: true
hosts:
- cert_expires: Apr  1 23:59:59 2027 GMT
  host: www.dcbel.energy
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Dcbel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dcbel, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Dcbel
provider_slug: dcbel
slug: dcbel-domain-security
source_filename: dcbel-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dcbel.energy\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  1 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: dcbel.energy\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/dcbel/security/dcbel-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- Cleantech
- Home Energy
- Solar
- Battery
---
