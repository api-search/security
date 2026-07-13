---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: vodafone.com
  spf: true
hosts:
- cert_expires: Sep 11 23:59:59 2026 GMT
  host: www.vodafone.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 10 14:02:50 2026 GMT
  host: developer.vodafone.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vodafone Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vodafone, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Vodafone
provider_slug: vodafone
slug: vodafone-domain-security
source_filename: vodafone-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.vodafone.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.vodafone.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 10 14:02:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: vodafone.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vodafone/refs/heads/main/security/vodafone-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Telecommunications
- Telco
- Mobile Network Operator
- 5G
- 4G
- Connectivity
- Broadband
- IoT
- Internet of Things
- Open Gateway
- CAMARA
- Network APIs
- Identity
- SIM Swap
- Number Verification
- Quality on Demand
- Quality of Service
- Roaming
- SMS
- Messaging
- Analytics
- Footfall
- Location
- Vodafone Business
- M-PESA
- Mobile Financial Services
- Enterprise
- Europe
- Africa
- United Kingdom
---
