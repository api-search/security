---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cubbystorage.com
  spf: true
hosts:
- cert_expires: Oct  5 20:21:26 2026 GMT
  host: www.cubbystorage.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  2 10:05:52 2026 GMT
  host: api.cubbystorage.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  hsts_note: 'Recorded as null by the automated probe because the API host root returns a JSON 404; a direct HEAD confirms ''strict-transport-security: max-age=31536000 ; includeSubDomains'' is served on every response from this host, including the 404 and the /mcp 401. Corrected by hand from the observed header on 2026-08-11.'
  https: true
  other_headers_observed:
  - x-content-type-options: nosniff
  - x-frame-options: DENY
  - x-xss-protection: '0'
  - 'cache-control: no-cache, no-store, max-age=0, must-revalidate'
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cubby Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cubby, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Cubby
provider_slug: cubby
slug: cubby-domain-security
source_filename: cubby-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cubbystorage.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 20:21:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.cubbystorage.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  2 10:05:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  hsts_note: >-\n    Recorded as null by the automated probe because the API host root returns a JSON 404; a\n    direct HEAD confirms 'strict-transport-security: max-age=31536000 ; includeSubDomains' is\n    served on every response from this host, including the 404 and the /mcp 401. Corrected\n    by hand from the observed header on 2026-08-11.\n  other_headers_observed:\n  - x-content-type-options: nosniff\n  - x-frame-options: DENY\n  - x-xss-protection: '0'\n  - 'cache-control: no-cache, no-store, max-age=0, must-revalidate'\ndomains:\n\
  - domain: cubbystorage.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cubby/refs/heads/main/security/cubby-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Self Storage
- Property Management
- Facility Management
- Real-Estate
- Payments
- Software-as-a-Service
- Artificial Intelligence
- Revenue Management
- E-Commerce
---
