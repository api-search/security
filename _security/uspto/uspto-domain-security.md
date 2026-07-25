---
api_specs:
- filename: uspto-assignments-api-openapi.yml
  format: yaml
  label: USPTO Assignments API
  slug: uspto-assignments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uspto/refs/heads/main/openapi/uspto-assignments-api-openapi.yml
- filename: uspto-patents-api-openapi.yml
  format: yaml
  label: USPTO Patents API
  slug: uspto-patents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uspto/refs/heads/main/openapi/uspto-patents-api-openapi.yml
- filename: uspto-ptab-api-openapi.yml
  format: yaml
  label: USPTO PTAB API
  slug: uspto-ptab-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uspto/refs/heads/main/openapi/uspto-ptab-api-openapi.yml
- filename: uspto-trademarks-api-openapi.yml
  format: yaml
  label: USPTO Trademarks API
  slug: uspto-trademarks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uspto/refs/heads/main/openapi/uspto-trademarks-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "digicert.com"
  - 0 issue "pki.goog"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: uspto.gov
  spf: true
hosts:
- cert_expires: Sep 19 04:00:00 2026 GMT
  host: developer.uspto.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
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
kind: domain-security
layout: security
method: probed
name: Uspto Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for USPTO, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: USPTO
provider_slug: uspto
slug: uspto-domain-security
source_filename: uspto-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.uspto.gov\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 19 04:00:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.uspto.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: data.uspto.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: uspto.gov\n  dnssec: true\n  caa:\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uspto/refs/heads/main/security/uspto-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC · DMARC
tags:
- Government
- Intellectual Property
- Open Data
- Patents
- Regulatory
- Trademarks
- USPTO
---
