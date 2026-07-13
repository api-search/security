---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: autonation.com
  spf: true
hosts:
- cert_expires: Oct  6 00:32:30 2026 GMT
  host: www.autonation.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Autonation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AutoNation, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: AutoNation
provider_slug: autonation
slug: autonation-domain-security
source_filename: autonation-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.autonation.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 00:32:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: autonation.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/autonation/refs/heads/main/security/autonation-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Automotive Retail
- Car Dealership
- Vehicle Sales
- Auto Finance
- Service Scheduling
- Used Vehicles
- Fortune 500
---
