---
api_specs:
- filename: uspto-patent-file-wrapper-openapi.yml
  format: yaml
  label: USPTO Patent File Wrapper API
  slug: uspto-patent-file-wrapper-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uspto-gov/refs/heads/main/openapi/uspto-patent-file-wrapper-openapi.yml
- filename: uspto-ptab-openapi.yml
  format: yaml
  label: USPTO Patent Trial and Appeal Board (PTAB) API
  slug: uspto-ptab-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uspto-gov/refs/heads/main/openapi/uspto-ptab-openapi.yml
- filename: uspto-tsdr-openapi.yml
  format: yaml
  label: USPTO Trademark Status and Document Retrieval (TSDR) API
  slug: uspto-tsdr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uspto-gov/refs/heads/main/openapi/uspto-tsdr-openapi.yml
- filename: uspto-office-actions-openapi.yml
  format: yaml
  label: USPTO Office Action APIs
  slug: uspto-office-action-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uspto-gov/refs/heads/main/openapi/uspto-office-actions-openapi.yml
- filename: uspto-bulk-data-openapi.yml
  format: yaml
  label: USPTO Bulk Data Storage System (BDSS) API
  slug: uspto-bulk-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uspto-gov/refs/heads/main/openapi/uspto-bulk-data-openapi.yml
- filename: uspto-patentsview-openapi.yml
  format: yaml
  label: USPTO PatentsView API
  slug: patentsview-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uspto-gov/refs/heads/main/openapi/uspto-patentsview-openapi.yml
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
