---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: americafirst.com
  spf: true
hosts:
- cert_expires: Sep 28 12:35:33 2026 GMT
  host: www.americafirst.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: America First Credit Union Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for America First Credit Union, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: America First Credit Union
provider_slug: america-first-credit-union
slug: america-first-credit-union-domain-security
source_filename: america-first-credit-union-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.americafirst.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 12:35:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: americafirst.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/america-first-credit-union/refs/heads/main/security/america-first-credit-union-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Financial-Services
- Banking
- United States
- Credit Union
- Consumer Banking
- Open Finance
- Data Aggregation
---
