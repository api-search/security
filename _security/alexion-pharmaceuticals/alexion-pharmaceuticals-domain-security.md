---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: alexion.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: astrazeneca.com
  spf: true
hosts:
- cert_expires: Dec 27 23:59:59 2026 GMT
  host: alexion.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  5 23:59:59 2026 GMT
  host: www.astrazeneca.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Alexion Pharmaceuticals Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for alexion-pharmaceuticals, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: alexion-pharmaceuticals
provider_slug: alexion-pharmaceuticals
slug: alexion-pharmaceuticals-domain-security
source_filename: alexion-pharmaceuticals-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: alexion.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 23:59:59 2026 GMT\n  hsts: false\n- host: www.astrazeneca.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  5 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: alexion.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: astrazeneca.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alexion-pharmaceuticals/refs/heads/main/security/alexion-pharmaceuticals-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Pharmaceuticals
- Rare Disease
- Biopharmaceutical
- Healthcare
- Genomics
- Complement Biology
- Hematology
- Neurology
---
