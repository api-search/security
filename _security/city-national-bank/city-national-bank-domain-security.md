---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cnb.com
  spf: true
hosts:
- cert_expires: Dec 24 23:59:59 2026 GMT
  host: www.cnb.com
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: City National Bank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for City National Bank, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: City National Bank
provider_slug: city-national-bank
slug: city-national-bank-domain-security
source_filename: city-national-bank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cnb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 86400\ndomains:\n- domain: cnb.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/city-national-bank/refs/heads/main/security/city-national-bank-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Financial-Services
- Banking
- United States
- Super-Regional Bank
- National Bank
- Private Banking
- Wealth Management
- Open Finance
- Data Aggregation
---
