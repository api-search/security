---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ascendtms.com
  spf: true
hosts:
- cert_expires: Dec  8 23:59:59 2026 GMT
  host: ascendtms.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: AscendTMS Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AscendTMS, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: AscendTMS
provider_slug: ascendtms
slug: ascendtms-domain-security
source_filename: ascendtms-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ascendtms.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: ascendtms.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/ascendtms/security/ascendtms-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Transportation
- Logistics
- Software-as-a-Service
- Freight
---
