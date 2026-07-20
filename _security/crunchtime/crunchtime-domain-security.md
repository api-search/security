---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: crunchtime.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: net-chef.com
  spf: true
hosts:
- cert_expires: Oct  7 20:28:51 2026 GMT
  host: developer.crunchtime.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 21:45:48 2026 GMT
  host: webservices.net-chef.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Crunchtime Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Crunchtime, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Crunchtime
provider_slug: crunchtime
slug: crunchtime-domain-security
source_filename: crunchtime-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.crunchtime.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 20:28:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: webservices.net-chef.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 21 21:45:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: crunchtime.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: net-chef.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crunchtime/refs/heads/main/security/crunchtime-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Restaurant Operations
- Inventory Management
- Labor & Scheduling
- Food Cost
- Kitchen Display
- Point of Sale
- Supply Chain
- Hospitality
- REST API
---
