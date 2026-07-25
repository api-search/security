---
api_specs:
- filename: uspto-gov-appeals-api-openapi.yml
  format: yaml
  label: USPTO Appeals API
  slug: uspto-gov-appeals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uspto-gov/refs/heads/main/openapi/uspto-gov-appeals-api-openapi.yml
- filename: uspto-gov-application-api-openapi.yml
  format: yaml
  label: USPTO Application API
  slug: uspto-gov-application-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uspto-gov/refs/heads/main/openapi/uspto-gov-application-api-openapi.yml
- filename: uspto-gov-assignments-api-openapi.yml
  format: yaml
  label: USPTO Assignments API
  slug: uspto-gov-assignments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uspto-gov/refs/heads/main/openapi/uspto-gov-assignments-api-openapi.yml
- filename: uspto-gov-citations-api-openapi.yml
  format: yaml
  label: USPTO Citations API
  slug: uspto-gov-citations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uspto-gov/refs/heads/main/openapi/uspto-gov-citations-api-openapi.yml
- filename: uspto-gov-datasets-api-openapi.yml
  format: yaml
  label: USPTO Datasets API
  slug: uspto-gov-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uspto-gov/refs/heads/main/openapi/uspto-gov-datasets-api-openapi.yml
- filename: uspto-gov-decisions-api-openapi.yml
  format: yaml
  label: USPTO Decisions API
  slug: uspto-gov-decisions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uspto-gov/refs/heads/main/openapi/uspto-gov-decisions-api-openapi.yml
- filename: uspto-gov-documents-api-openapi.yml
  format: yaml
  label: USPTO Documents API
  slug: uspto-gov-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uspto-gov/refs/heads/main/openapi/uspto-gov-documents-api-openapi.yml
- filename: uspto-gov-enriched-citations-api-openapi.yml
  format: yaml
  label: USPTO Enriched Citations API
  slug: uspto-gov-enriched-citations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uspto-gov/refs/heads/main/openapi/uspto-gov-enriched-citations-api-openapi.yml
- filename: uspto-gov-office-actions-api-openapi.yml
  format: yaml
  label: USPTO Office Actions API
  slug: uspto-gov-office-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uspto-gov/refs/heads/main/openapi/uspto-gov-office-actions-api-openapi.yml
- filename: uspto-gov-patentsview-api-openapi.yml
  format: yaml
  label: USPTO Patentsview API
  slug: uspto-gov-patentsview-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uspto-gov/refs/heads/main/openapi/uspto-gov-patentsview-api-openapi.yml
- filename: uspto-gov-proceedings-api-openapi.yml
  format: yaml
  label: USPTO Proceedings API
  slug: uspto-gov-proceedings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uspto-gov/refs/heads/main/openapi/uspto-gov-proceedings-api-openapi.yml
- filename: uspto-gov-rejections-api-openapi.yml
  format: yaml
  label: USPTO Rejections API
  slug: uspto-gov-rejections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uspto-gov/refs/heads/main/openapi/uspto-gov-rejections-api-openapi.yml
- filename: uspto-gov-search-api-openapi.yml
  format: yaml
  label: USPTO Search API
  slug: uspto-gov-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uspto-gov/refs/heads/main/openapi/uspto-gov-search-api-openapi.yml
- filename: uspto-gov-status-api-openapi.yml
  format: yaml
  label: USPTO Status API
  slug: uspto-gov-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uspto-gov/refs/heads/main/openapi/uspto-gov-status-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "digicert.com"
  - 0 issue "pki.goog"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: uspto.gov
  spf: true
hosts:
- cert_expires: Oct  1 23:59:59 2026 GMT
  host: www.uspto.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 11 23:59:59 2026 GMT
  host: data.uspto.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 04:00:00 2026 GMT
  host: developer.uspto.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Uspto Gov Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for USPTO, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: USPTO
provider_slug: uspto-gov
slug: uspto-gov-domain-security
source_filename: uspto-gov-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.uspto.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: data.uspto.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.uspto.gov\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 19 04:00:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: uspto.gov\n  dnssec: true\n  caa:\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uspto-gov/refs/heads/main/security/uspto-gov-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Patents
- Trademarks
- Intellectual Property
- Government
- Federal
- Open Data
- PTAB
- TSDR
---
