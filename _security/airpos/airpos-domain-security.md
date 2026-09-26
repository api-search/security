---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: airpointofsale.com
  spf: true
hosts:
- cert_expires: Oct 29 07:42:18 2026 GMT
  host: www.airpointofsale.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Airpos Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AirPOS, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: AirPOS
provider_slug: airpos
slug: airpos-domain-security
source_filename: airpos-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.airpointofsale.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 07:42:18 2026 GMT\n  hsts: false\ndomains:\n- domain: airpointofsale.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/airpos/refs/heads/main/security/airpos-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Point-of-Sale
- Retail
- Payments
- Inventory
- E-Commerce
- United Kingdom
- Northern Ireland
---
