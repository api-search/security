---
api_specs:
- filename: sorsa-community-api-openapi.yml
  format: yaml
  label: Sorsa Community API
  slug: sorsa-community-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sorsa/refs/heads/main/openapi/sorsa-community-api-openapi.yml
- filename: sorsa-lists-api-openapi.yml
  format: yaml
  label: Sorsa Lists API
  slug: sorsa-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sorsa/refs/heads/main/openapi/sorsa-lists-api-openapi.yml
- filename: sorsa-search-api-openapi.yml
  format: yaml
  label: Sorsa Search API
  slug: sorsa-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sorsa/refs/heads/main/openapi/sorsa-search-api-openapi.yml
- filename: sorsa-sorsa-info-crypto-related-api-openapi.yml
  format: yaml
  label: Sorsa Sorsa Info Crypto Related API
  slug: sorsa-sorsa-info-crypto-related-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sorsa/refs/heads/main/openapi/sorsa-sorsa-info-crypto-related-api-openapi.yml
- filename: sorsa-technical-endpoints-api-openapi.yml
  format: yaml
  label: Sorsa Technical Endpoints API
  slug: sorsa-technical-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sorsa/refs/heads/main/openapi/sorsa-technical-endpoints-api-openapi.yml
- filename: sorsa-tweets-api-openapi.yml
  format: yaml
  label: Sorsa Tweets API
  slug: sorsa-tweets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sorsa/refs/heads/main/openapi/sorsa-tweets-api-openapi.yml
- filename: sorsa-users-data-api-openapi.yml
  format: yaml
  label: Sorsa Users Data API
  slug: sorsa-users-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sorsa/refs/heads/main/openapi/sorsa-users-data-api-openapi.yml
- filename: sorsa-verification-api-openapi.yml
  format: yaml
  label: Sorsa Verification API
  slug: sorsa-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sorsa/refs/heads/main/openapi/sorsa-verification-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: sorsa.io
  spf: true
hosts:
- cert_expires: Sep 16 04:51:34 2026 GMT
  host: sorsa.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 04:51:34 2026 GMT
  host: docs.sorsa.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 06:25:00 2026 GMT
  host: api.sorsa.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sorsa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sorsa, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Sorsa
provider_slug: sorsa
slug: sorsa-domain-security
source_filename: sorsa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sorsa.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 04:51:34 2026 GMT\n  hsts: false\n- host: docs.sorsa.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 04:51:34 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.sorsa.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 06:25:00 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: sorsa.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sorsa/refs/heads/main/security/sorsa-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Twitter
- X
- Social-Media
- Data Extraction
- Real-Time
---
