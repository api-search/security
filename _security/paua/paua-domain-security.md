---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: paua.com
  spf: false
hosts:
- cert_expires: Sep 28 18:29:43 2026 GMT
  host: www.paua.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Paua Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Paua, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Paua
provider_slug: paua
slug: paua-domain-security
source_filename: paua-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.paua.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 18:29:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: paua.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paua/refs/heads/main/security/paua-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- EV Charging
- Electric Vehicles
- Fleet Management
- Mobility
- Payments
- Energy
- Charge Card
- United Kingdom
---
