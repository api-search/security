---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: fnb-online.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: plaid.com
  spf: true
hosts:
- cert_expires: Nov 11 23:59:59 2026 GMT
  host: www.fnb-online.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct 13 23:59:59 2026 GMT
  host: plaid.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fnb Corp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for F.N.B. Corporation, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: F.N.B. Corporation
provider_slug: fnb-corp
slug: fnb-corp-domain-security
source_filename: fnb-corp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fnb-online.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 11 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: plaid.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: fnb-online.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: plaid.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fnb-corp/refs/heads/main/security/fnb-corp-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC · DMARC
tags:
- Financial-Services
- Banking
- United States
- Regional Bank
- Consumer Banking
- Commercial Banking
- Wealth Management
- Data Aggregation
- Open Finance
---
