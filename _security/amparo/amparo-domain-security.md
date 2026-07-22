---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: amparo.com.vc
  spf: true
hosts:
- cert_expires: Oct 13 23:14:02 2026 GMT
  host: www.amparo.com.vc
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Amparo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amparo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Amparo
provider_slug: amparo
slug: amparo-domain-security
source_filename: amparo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.amparo.com.vc\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 23:14:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: amparo.com.vc\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amparo/refs/heads/main/security/amparo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Brazil
- Financial Services
- Insurance
- Lending
- Bereavement
- Document Processing
---
