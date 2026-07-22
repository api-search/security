---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: 2ulaundry.com
  spf: true
hosts:
- cert_expires: Sep 24 23:03:02 2026 GMT
  host: 2ulaundry.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: 2Ulaundry Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 2ULaundry, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: 2ULaundry
provider_slug: 2ulaundry
slug: 2ulaundry-domain-security
source_filename: 2ulaundry-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 2ulaundry.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 23:03:02 2026 GMT\n  hsts: false\ndomains:\n- domain: 2ulaundry.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/2ulaundry/refs/heads/main/security/2ulaundry-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Laundry
- Dry Cleaning
- Delivery
- Logistics
- Consumer Services
- On-Demand
---
