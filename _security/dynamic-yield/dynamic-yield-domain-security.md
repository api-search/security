---
api_specs:
- filename: dynamic-yield-api-only-api-openapi.yml
  format: yaml
  label: Dynamic Yield API only API
  slug: dynamic-yield-api-only-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynamic-yield/refs/heads/main/openapi/dynamic-yield-api-only-api-openapi.yml
- filename: dynamic-yield-experience-apis-api-openapi.yml
  format: yaml
  label: Dynamic Yield Experience APIs API
  slug: dynamic-yield-experience-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynamic-yield/refs/heads/main/openapi/dynamic-yield-experience-apis-api-openapi.yml
- filename: dynamic-yield-product-data-api-openapi.yml
  format: yaml
  label: Dynamic Yield Product Data API
  slug: dynamic-yield-product-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynamic-yield/refs/heads/main/openapi/dynamic-yield-product-data-api-openapi.yml
- filename: dynamic-yield-profile-anywhere-api-openapi.yml
  format: yaml
  label: Dynamic Yield Profile Anywhere API
  slug: dynamic-yield-profile-anywhere-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynamic-yield/refs/heads/main/openapi/dynamic-yield-profile-anywhere-api-openapi.yml
- filename: dynamic-yield-user-data-api-api-openapi.yml
  format: yaml
  label: Dynamic Yield User Data API
  slug: dynamic-yield-user-data-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynamic-yield/refs/heads/main/openapi/dynamic-yield-user-data-api-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: dynamicyield.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: dy.dev
  spf: true
hosts:
- cert_expires: Oct 15 11:30:14 2026 GMT
  host: www.dynamicyield.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 30 07:16:49 2026 GMT
  host: dy.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 18 23:59:59 2027 GMT
  host: dy-api.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Dynamic Yield Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dynamic Yield, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Dynamic Yield
provider_slug: dynamic-yield
slug: dynamic-yield-domain-security
source_filename: dynamic-yield-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dynamicyield.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 11:30:14 2026 GMT\n  hsts: false\n- host: dy.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 07:16:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: dy-api.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 18 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: dynamicyield.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: dy.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dynamic-yield/refs/heads/main/security/dynamic-yield-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Cloud
- Personalization
- Experience Optimization
- Recommendations
- A/B Testing
- Search
- E-Commerce
- Retail
- Machine Learning
- MACH
- Mastercard
---
