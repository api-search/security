---
api_specs:
- filename: swagger.yaml
  format: yaml
  label: USPTO Open Data Portal API
  slug: open-data-portal-api
  spec_type: OpenAPI
  url: https://data.uspto.gov/swagger/swagger.yaml
- filename: uspto-tsdr-openapi.yml
  format: yaml
  label: USPTO Trademark Status and Document Retrieval API
  slug: tsdr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-patent-and-trademark-office/refs/heads/main/openapi/uspto-tsdr-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "digicert.com"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: uspto.gov
  spf: true
hosts:
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
- cert_expires: Dec 11 23:59:59 2026 GMT
  host: api.uspto.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Us Patent And Trademark Office Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for US Patent and Trademark Office, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: US Patent and Trademark Office
provider_slug: us-patent-and-trademark-office
slug: us-patent-and-trademark-office-domain-security
source_filename: us-patent-and-trademark-office-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: data.uspto.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.uspto.gov\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 19 04:00:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.uspto.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: uspto.gov\n  dnssec: true\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/us-patent-and-trademark-office/refs/heads/main/security/us-patent-and-trademark-office-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Federal Government
- Patents
- Trademarks
- Intellectual Property
- Open Data
---
