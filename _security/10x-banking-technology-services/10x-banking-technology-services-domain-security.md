---
api_specs:
- filename: overview
  format: yaml
  label: 10x Banking Platform API
  slug: 10x-banking-platform-api
  spec_type: Postman
  url: https://www.postman.com/openbanking10x/10x-banking-public-workspace/overview
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: 10xbanking.com
  spf: true
hosts:
- cert_expires: Nov 13 15:40:53 2026 GMT
  host: www.10xbanking.com
  hsts: true
  hsts_max_age: 3628800
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  5 18:43:31 2026 GMT
  host: docs.10xbanking.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 21 23:59:59 2026 GMT
  host: api.sandbox.10xbanking.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  hsts_note: 'Corrected by hand from a direct probe on 2026-09-05. The automated pass recorded null because every response on this host is a 401; the 401 itself carries strict-transport-security: max-age=31536000; includeSubDomains, confirmed on three consecutive requests.'
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: 10X Banking Technology Services Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 10x Banking Technology Services, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: 10x Banking Technology Services
provider_slug: 10x-banking-technology-services
slug: 10x-banking-technology-services-domain-security
source_filename: 10x-banking-technology-services-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.10xbanking.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 13 15:40:53 2026 GMT\n  hsts: true\n  hsts_max_age: 3628800\n- host: docs.10xbanking.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  5 18:43:31 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.sandbox.10xbanking.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 21 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  hsts_note: >-\n    Corrected by hand from a direct probe on 2026-09-05. The automated pass recorded\n    null because every response on this host is a 401; the 401 itself carries\n    strict-transport-security: max-age=31536000; includeSubDomains, confirmed on three\n    consecutive requests.\ndomains:\n- domain: 10xbanking.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n\
  \  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/10x-banking-technology-services/refs/heads/main/security/10x-banking-technology-services-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Financial-Services
- Banking
- Core Banking
- Cloud Native
- Banking as a Service
- Embedded Finance
- Payments
- Lending
- Deposits
- Cards
- Event Driven
- United Kingdom
- SaaS
- Fintech
---
