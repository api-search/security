---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: x4pharma.com
  spf: true
hosts:
- cert_expires: Dec 22 07:01:16 2026 GMT
  host: www.x4pharma.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: X4 Pharmaceuticals Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for X4 Pharmaceuticals, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: X4 Pharmaceuticals
provider_slug: x4-pharmaceuticals
slug: x4-pharmaceuticals-domain-security
source_filename: x4-pharmaceuticals-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.x4pharma.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 07:01:16 2026 GMT\n  hsts: false\ndomains:\n- domain: x4pharma.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/x4-pharmaceuticals/security/x4-pharmaceuticals-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Biotechnology
- Pharmaceuticals
- Rare Diseases
- Clinical Trials
---
