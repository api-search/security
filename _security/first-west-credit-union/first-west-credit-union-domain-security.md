---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: trucooperativebank.ca
  spf: true
hosts:
- cert_expires: Jan  7 23:59:59 2027 GMT
  host: www.trucooperativebank.ca
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: First West Credit Union Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for First West Credit Union, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: First West Credit Union
provider_slug: first-west-credit-union
slug: first-west-credit-union-domain-security
source_filename: first-west-credit-union-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.trucooperativebank.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31557600\ndomains:\n- domain: trucooperativebank.ca\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/first-west-credit-union/refs/heads/main/security/first-west-credit-union-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Financial-Services
- Banking
- Canada
- Credit Union
- Cooperative Bank
- British Columbia
- Consumer-Driven Banking
- Data Aggregation
---
