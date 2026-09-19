---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: aero-tech.com.cn
  spf: true
hosts:
- cert_expires: Mar 11 23:59:59 2027 GMT
  host: www.aero-tech.com.cn
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aerotech388E Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aerotech (Beijing), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Aerotech (Beijing)
provider_slug: aerotech388e
slug: aerotech388e-domain-security
source_filename: aerotech388e-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.aero-tech.com.cn\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 11 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: aero-tech.com.cn\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aerotech388e/refs/heads/main/security/aerotech388e-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Semiconductors
- Manufacturing
- Hardware
- Industrial Equipment
- Valves
- Gas Delivery
- Ultra High Purity
- Electropolishing
- China
---
