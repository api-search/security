---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: kddi.com
  spf: true
hosts:
- cert_expires: Nov  4 06:11:01 2026 GMT
  host: www.kddi.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Kddi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for KDDI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: KDDI
provider_slug: kddi
slug: kddi-domain-security
source_filename: kddi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kddi.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  4 06:11:01 2026 GMT\n  hsts: false\ndomains:\n- domain: kddi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kddi/refs/heads/main/security/kddi-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Telecommunications
- Mobile Network Operator
- Carrier
- Japan
- au
- UQ Mobile
- povo
- Network API
- CAMARA
- Aduna
- Identity Verification
- Consent Management
- Mini App
- au PAY
- XR
- MEC
- Edge Computing
- 5G
- Cloud Platform
- IoT
---
