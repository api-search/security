---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: fiserv.com
  spf: true
hosts:
- host: www.fiserv.com
  https: false
- cert_expires: Jan 21 23:59:59 2027 GMT
  host: developer.fiserv.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: First Data Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for First Data (Fiserv), probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: First Data (Fiserv)
provider_slug: first-data
slug: first-data-domain-security
source_filename: first-data-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fiserv.com\n  https: false\n- host: developer.fiserv.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 21 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: fiserv.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/first-data/refs/heads/main/security/first-data-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Payments
- Merchant Services
- Financial-Services
- Transaction Processing
- Fortune 500
---
