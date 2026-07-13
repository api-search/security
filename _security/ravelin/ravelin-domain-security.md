---
api_specs:
- filename: ravelin-merchant-api-openapi.yml
  format: yaml
  label: Ravelin Merchant API
  slug: ravelin-merchant-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ravelin/refs/heads/main/openapi/ravelin-merchant-api-openapi.yml
- filename: ravelin-3ds-server-api-openapi.yml
  format: yaml
  label: Ravelin 3D Secure Server API
  slug: ravelin-3ds-server-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ravelin/refs/heads/main/openapi/ravelin-3ds-server-api-openapi.yml
- filename: ravelin-callbacks-api-openapi.yml
  format: yaml
  label: Ravelin Callbacks API
  slug: ravelin-callbacks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ravelin/refs/heads/main/openapi/ravelin-callbacks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: ravelin.com
  spf: true
hosts:
- cert_expires: Sep 20 07:18:05 2026 GMT
  host: www.ravelin.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 10:49:22 2026 GMT
  host: developer.ravelin.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 15 23:59:59 2026 GMT
  host: api.ravelin.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ravelin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ravelin, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Ravelin
provider_slug: ravelin
slug: ravelin-domain-security
source_filename: ravelin-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ravelin.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 07:18:05 2026 GMT\n  hsts: false\n- host: developer.ravelin.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 10:49:22 2026 GMT\n  hsts: false\n- host: api.ravelin.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: ravelin.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ravelin/refs/heads/main/security/ravelin-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Fraud Prevention
- Fraud Detection
- Chargeback Prevention
- Account Takeover
- 3D Secure
- Risk Scoring
- Payments
- Machine Learning
---
