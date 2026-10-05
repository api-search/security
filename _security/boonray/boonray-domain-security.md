---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: boonray.com
  spf: false
hosts:
- cert_expires: Nov 21 15:36:05 2026 GMT
  host: en.boonray.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Boonray Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Boonray, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Boonray
provider_slug: boonray
slug: boonray-domain-security
source_filename: boonray-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: en.boonray.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 21 15:36:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: boonray.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/boonray/refs/heads/main/security/boonray-domain-security.yml
summary_line: TLSv1.2 · HSTS
tags:
- Company
- Autonomous Driving
- MiningTech
- SmartCars
- New Energy
---
