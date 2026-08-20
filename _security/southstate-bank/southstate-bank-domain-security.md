---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: southstatebank.com
  spf: true
hosts:
- cert_expires: Oct 11 04:15:17 2026 GMT
  host: www.southstatebank.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Southstate Bank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SouthState Bank, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: SouthState Bank
provider_slug: southstate-bank
slug: southstate-bank-domain-security
source_filename: southstate-bank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.southstatebank.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 11 04:15:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: southstatebank.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/southstate-bank/refs/heads/main/security/southstate-bank-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC · DMARC
tags:
- Financial-Services
- Banking
- United States
- Regional Bank
- National Bank
- Open Finance
- Data Aggregation
---
