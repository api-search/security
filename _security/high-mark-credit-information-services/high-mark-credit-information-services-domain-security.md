---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: crifhighmark.com
  spf: true
hosts:
- cert_expires: Aug 21 11:19:36 2026 GMT
  host: www.crifhighmark.com
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: High Mark Credit Information Services Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for High Mark Credit Information Services, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: High Mark Credit Information Services
provider_slug: high-mark-credit-information-services
slug: high-mark-credit-information-services-domain-security
source_filename: high-mark-credit-information-services-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.crifhighmark.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 11:19:36 2026 GMT\n  hsts: true\n  hsts_max_age: 86400\ndomains:\n- domain: crifhighmark.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/high-mark-credit-information-services/refs/heads/main/security/high-mark-credit-information-services-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Credit Bureau
- Credit Information
- Credit Scoring
- Financial Services
- Risk Analytics
- Microfinance
- Lending
- India
---
