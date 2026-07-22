---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ubereats.com
  spf: true
hosts:
- cert_expires: Feb 16 23:59:59 2027 GMT
  host: www.ubereats.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cornershop Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cornershop by Uber, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Cornershop by Uber
provider_slug: cornershop
slug: cornershop-domain-security
source_filename: cornershop-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ubereats.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 16 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: ubereats.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cornershop/refs/heads/main/security/cornershop-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Grocery Delivery
- On-Demand Delivery
- Last Mile Delivery
- Consumer Apps
- E-Commerce
- Marketplaces
- Logistics
- Latin America
- Chile
- Mexico
- Uber
- Uber Eats
- Acquired
- Retail
---
