---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: ozk.com
  spf: true
hosts:
- cert_expires: Mar 13 17:02:11 2027 GMT
  host: www.ozk.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bank Ozk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bank OZK, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Bank OZK
provider_slug: bank-ozk
slug: bank-ozk-domain-security
source_filename: bank-ozk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ozk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 13 17:02:11 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ozk.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bank-ozk/refs/heads/main/security/bank-ozk-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Financial Services
- Banking
- United States
- Regional Bank
- Commercial Real Estate Lending
- Open Finance
- Data Aggregation
---
