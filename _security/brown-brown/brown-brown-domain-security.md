---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bbrown.com
  spf: true
hosts:
- cert_expires: Sep  3 00:43:50 2026 GMT
  host: www.bbrown.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 22:42:30 2026 GMT
  host: us.bbrown.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Brown Brown Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Brown & Brown, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Brown & Brown
provider_slug: brown-brown
slug: brown-brown-domain-security
source_filename: brown-brown-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bbrown.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 00:43:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: us.bbrown.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 22:42:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bbrown.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brown-brown/refs/heads/main/security/brown-brown-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Insurance
- United States
- Broker
- Property and Casualty
- Employee Benefits
- Wholesale Brokerage
- Managing General Agent
- Risk Management
- Agency Management
- Partner Gated
---
