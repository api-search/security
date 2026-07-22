---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: trycaviar.com
  spf: true
hosts:
- cert_expires: Oct 15 01:46:22 2026 GMT
  host: www.trycaviar.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Caviar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Caviar, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Caviar
provider_slug: caviar
slug: caviar-domain-security
source_filename: caviar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.trycaviar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 01:46:22 2026 GMT\n  hsts: null\ndomains:\n- domain: trycaviar.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/caviar/refs/heads/main/security/caviar-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Food Delivery
- Restaurants
- Marketplace
- Logistics
- On-Demand
- Ordering
- Catering
---
