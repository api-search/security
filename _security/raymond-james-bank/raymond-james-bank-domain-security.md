---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: raymondjamesbank.com
  spf: true
hosts:
- cert_expires: Dec 17 23:59:59 2026 GMT
  host: www.raymondjamesbank.com
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Raymond James Bank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Raymond James Bank, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Raymond James Bank
provider_slug: raymond-james-bank
slug: raymond-james-bank-domain-security
source_filename: raymond-james-bank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.raymondjamesbank.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 86400\ndomains:\n- domain: raymondjamesbank.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/raymond-james-bank/refs/heads/main/security/raymond-james-bank-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Financial-Services
- Banking
- United States
- Wealth Management
- Securities-Based Lending
- Open Finance
- Data Aggregation
---
