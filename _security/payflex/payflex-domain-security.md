---
api_specs:
- filename: payflex-authentication-api-openapi.yml
  format: yaml
  label: Payflex Authentication API
  slug: payflex-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payflex/refs/heads/main/openapi/payflex-authentication-api-openapi.yml
- filename: payflex-configuration-api-openapi.yml
  format: yaml
  label: Payflex Configuration API
  slug: payflex-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payflex/refs/heads/main/openapi/payflex-configuration-api-openapi.yml
- filename: payflex-orders-api-openapi.yml
  format: yaml
  label: Payflex Orders API
  slug: payflex-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payflex/refs/heads/main/openapi/payflex-orders-api-openapi.yml
- filename: payflex-refunds-api-openapi.yml
  format: yaml
  label: Payflex Refunds API
  slug: payflex-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payflex/refs/heads/main/openapi/payflex-refunds-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: payflex.co.za
  spf: true
hosts:
- cert_expires: Sep  6 13:44:59 2026 GMT
  host: payflex.co.za
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 17 14:15:32 2026 GMT
  host: docs.payflex.co.za
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  6 13:44:59 2026 GMT
  host: api.payflex.co.za
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Payflex Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Payflex, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Payflex
provider_slug: payflex
slug: payflex-domain-security
source_filename: payflex-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: payflex.co.za\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 13:44:59 2026 GMT\n  hsts: false\n- host: docs.payflex.co.za\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 14:15:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.payflex.co.za\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 13:44:59 2026 GMT\n  hsts: false\ndomains:\n- domain: payflex.co.za\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/payflex/refs/heads/main/security/payflex-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- BNPL
- Buy Now Pay Later
- Payments
- Installments
- South Africa
- Fintech
- E-Commerce
---
