---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: glia.com
  spf: true
  spf_record: v=spf1 include:_spf.google.com include:amazonses.com include:mktomail.com include:stspg-customer.com include:spf.protection.outlook.com include:sendgrid.net ~all
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: glia.eu
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: salemove.com
  spf: true
hosts:
- cert_expires: Sep 26 13:46:34 2026 GMT
  host: www.glia.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  hsts_preload: true
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  6 09:18:37 2026 GMT
  host: docs.glia.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 63072000
  hsts_preload: true
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 23:59:59 2026 GMT
  host: api.glia.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  hsts_preload: false
  https: true
  note: observed on the 401 response to GET /operators; the host root itself returns 404
  tls_version: TLSv1.3
- host: api.glia.eu
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  hsts_preload: false
  https: true
  tls_version: TLSv1.3
- host: sdk-docs.glia.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  hsts_preload: false
  https: true
- host: status.glia.com
  hsts: true
  hsts_include_subdomains: false
  hsts_max_age: 259200
  hsts_preload: false
  https: true
kind: domain-security
layout: security
method: probed
name: Glia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Glia, probed live across 6 host(s) and 3 registrable domain(s). 6 host(s) serve HTTPS (up to TLSv1.3); 6 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Glia
provider_slug: glia
slug: glia-domain-security
source_filename: glia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml hosts (probe-domain-security.py + manual header probe)\nhosts:\n- host: www.glia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 13:46:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  hsts_preload: true\n- host: docs.glia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 09:18:37 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n  hsts_include_subdomains: true\n  hsts_preload: true\n- host: api.glia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  hsts_preload: false\n  note: observed on the 401 response to GET /operators; the host root itself returns 404\n- host: api.glia.eu\n  https: true\n  tls_version: TLSv1.3\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  hsts_preload: false\n\
  - host: sdk-docs.glia.com\n  https: true\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  hsts_preload: false\n- host: status.glia.com\n  https: true\n  hsts: true\n  hsts_max_age: 259200\n  hsts_include_subdomains: false\n  hsts_preload: false\ndomains:\n- domain: glia.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 include:_spf.google.com include:amazonses.com include:mktomail.com\n    include:stspg-customer.com include:spf.protection.outlook.com include:sendgrid.net ~all\n  dmarc: true\n  dmarc_policy: reject\n- domain: glia.eu\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n- domain: salemove.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\nx-evidence:\n  fetched: '2026-08-04'\n  tools:\n  - dig\n  - curl -D\n  notes: >-\n    No CAA records are published on any Glia registrable domain and none are DNSSEC signed.\n    glia.eu carries a DMARC record at p=none (monitor only)\
  \ and publishes no SPF record,\n    while glia.com and salemove.com are both at p=reject with SPF.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/glia/refs/heads/main/security/glia-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Customer Service
- Contact Center
- Banking
- Credit Unions
- Financial-Services
- Conversational AI
- Voice
- CoBrowsing
- Serverless
---
