---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: glia.com
  spf: true
hosts:
- cert_expires: Sep 26 13:46:34 2026 GMT
  host: www.glia.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Glia Fka Salemove Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Glia (fka SaleMove), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Glia (fka SaleMove)
provider_slug: glia-fka-salemove
slug: glia-fka-salemove-domain-security
source_filename: glia-fka-salemove-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.glia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 13:46:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: glia.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/glia-fka-salemove/refs/heads/main/security/glia-fka-salemove-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Customer Service
- Customer Support
- Digital Customer Service
- Contact Center
- Conversational AI
- Voice AI
- Co-Browsing
- Financial Services
- Banking
- Serverless
- SDK
---
