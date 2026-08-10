---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: csair.com
  spf: true
hosts:
- cert_expires: Oct 11 23:59:59 2026 GMT
  host: cargo.csair.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: China Southern Air Logistics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for China Southern Air Logistics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: China Southern Air Logistics
provider_slug: china-southern-air-logistics
slug: china-southern-air-logistics-domain-security
source_filename: china-southern-air-logistics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cargo.csair.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 11 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: csair.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/china-southern-air-logistics/refs/heads/main/security/china-southern-air-logistics-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Air Cargo
- Air Freight
- Logistics
- Freight
- Shipping
- Transportation
- Supply Chain
- Aviation
- China
- Cargo Tracking
---
