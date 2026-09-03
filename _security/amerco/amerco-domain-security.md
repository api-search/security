---
api_specs:
- filename: amerco-webselfstorage-affiliate-api-v4-openapi.yml
  format: yaml
  label: WebSelfStorage Affiliate API
  slug: webselfstorage
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amerco/refs/heads/main/openapi/amerco-webselfstorage-affiliate-api-v4-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: amerco.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: uhaul.com
  spf: true
hosts:
- cert_expires: Oct  7 21:15:38 2026 GMT
  host: www.amerco.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 12 23:59:59 2026 GMT
  host: www.uhaul.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Dec 20 23:59:59 2026 GMT
  host: api.webselfstorage.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  hsts_note: 'Corrected by hand 2026-09-02. probe-domain-security.py recorded hsts: null because the host root returns a Swagger UI shell; a live GET https://api.webselfstorage.com/v4/test (HTTP 401) and a HEAD of the root both returned "Strict-Transport-Security: max-age=31536000; includeSubDomains".'
  https: true
  other_headers_observed:
  - X-Content-Type-Options
  - X-XSS-Protection
  - Content-Security-Policy
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Amerco Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AMERCO, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: AMERCO
provider_slug: amerco
slug: amerco-domain-security
source_filename: amerco-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.amerco.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 21:15:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.uhaul.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 12 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.webselfstorage.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 20 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  hsts_note: >-\n    Corrected by hand 2026-09-02. probe-domain-security.py recorded hsts: null because the\n    host root returns a Swagger UI shell; a live GET https://api.webselfstorage.com/v4/test\n    (HTTP 401) and a HEAD of the root both returned\n    \"Strict-Transport-Security: max-age=31536000; includeSubDomains\".\n  other_headers_observed: [X-Content-Type-Options, X-XSS-Protection, Content-Security-Policy]\n\
  domains:\n- domain: amerco.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: uhaul.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amerco/refs/heads/main/security/amerco-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Moving
- Storage
- Truck Rental
- Logistics
- Consumer Services
- Fortune 1000
---
