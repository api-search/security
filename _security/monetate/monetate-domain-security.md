---
api_specs:
- filename: monetate-engine-api-openapi.yml
  format: yaml
  label: Monetate Engine API
  slug: monetate-engine-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monetate/refs/heads/main/openapi/monetate-engine-api-openapi.yml
- filename: monetate-data-api-openapi.yml
  format: yaml
  label: Monetate Data API
  slug: monetate-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monetate/refs/heads/main/openapi/monetate-data-api-openapi.yml
- filename: monetate-metadata-api-openapi.yml
  format: yaml
  label: Monetate Metadata API
  slug: monetate-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monetate/refs/heads/main/openapi/monetate-metadata-api-openapi.yml
- filename: monetate-auth-api-openapi.yml
  format: yaml
  label: Monetate Auth API
  slug: monetate-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monetate/refs/heads/main/openapi/monetate-auth-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: monetate.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: monetate.net
  spf: false
hosts:
- cert_expires: Sep 25 22:31:51 2026 GMT
  host: monetate.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 18:41:01 2026 GMT
  host: developer.monetate.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 23 23:59:59 2027 GMT
  host: engine.monetate.net
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Monetate Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Monetate, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Monetate
provider_slug: monetate
slug: monetate-domain-security
source_filename: monetate-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: monetate.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 22:31:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.monetate.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 18:41:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: engine.monetate.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 23 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: monetate.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: monetate.net\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/monetate/refs/heads/main/security/monetate-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Personalization
- Experience Optimization
- A/B Testing
- Ecommerce
- Product Recommendations
- Personalized Search
- Marketing
- Customer Data
- Retail
- Decision Engine
---
