---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ieso.ca
  spf: true
hosts:
- cert_expires: Dec 16 23:59:59 2026 GMT
  host: www.ieso.ca
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 18 23:59:59 2026 GMT
  host: reports-public.ieso.ca
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct 22 23:59:59 2026 GMT
  host: reports.ieso.ca
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Ieso Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for IESO, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: IESO
provider_slug: ieso
slug: ieso-domain-security
source_filename: ieso-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ieso.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 23:59:59 2026 GMT\n  hsts: false\n- host: reports-public.ieso.ca\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 18 23:59:59 2026 GMT\n  hsts: false\n- host: reports.ieso.ca\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 22 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\ndomains:\n- domain: ieso.ca\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ieso/refs/heads/main/security/ieso-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- Canada
- Electricity
- Energy Markets
- Grid
- System Operator
- Market Data
- Open Data
- Ontario
- Demand Response
- Renewables
---
