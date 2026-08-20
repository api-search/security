---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: santanderbank.com
  spf: true
hosts:
- cert_expires: Dec 18 23:59:59 2026 GMT
  host: www.santanderbank.com
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Santander Us Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Santander US, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Santander US
provider_slug: santander-us
slug: santander-us-domain-security
source_filename: santander-us-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.santanderbank.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 86400\ndomains:\n- domain: santanderbank.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/santander-us/refs/heads/main/security/santander-us-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Financial-Services
- Banking
- United States
- Super-Regional Bank
- Retail Banking
- Open Finance
- Data Aggregation
---
