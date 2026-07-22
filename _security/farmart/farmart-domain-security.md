---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: farmart.co
  spf: true
hosts:
- cert_expires: Sep 24 15:25:33 2026 GMT
  host: farmart.co
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Farmart Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FarMart, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: FarMart
provider_slug: farmart
slug: farmart-domain-security
source_filename: farmart-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: farmart.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 15:25:33 2026 GMT\n  hsts: false\ndomains:\n- domain: farmart.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/farmart/refs/heads/main/security/farmart-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Agriculture
- AgriTech
- Food Supply Chain
- Procurement
- Payments
- Traceability
- Logistics
---
