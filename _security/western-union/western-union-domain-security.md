---
api_specs:
- filename: western-union-balances-api-openapi.yml
  format: yaml
  label: western-union Balances API
  slug: western-union-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/western-union/refs/heads/main/openapi/western-union-balances-api-openapi.yml
- filename: western-union-batches-api-openapi.yml
  format: yaml
  label: western-union Batches API
  slug: western-union-batches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/western-union/refs/heads/main/openapi/western-union-batches-api-openapi.yml
- filename: western-union-customers-api-openapi.yml
  format: yaml
  label: western-union Customers API
  slug: western-union-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/western-union/refs/heads/main/openapi/western-union-customers-api-openapi.yml
- filename: western-union-health-api-openapi.yml
  format: yaml
  label: western-union Health API
  slug: western-union-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/western-union/refs/heads/main/openapi/western-union-health-api-openapi.yml
- filename: western-union-orders-api-openapi.yml
  format: yaml
  label: western-union Orders API
  slug: western-union-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/western-union/refs/heads/main/openapi/western-union-orders-api-openapi.yml
- filename: western-union-payments-api-openapi.yml
  format: yaml
  label: western-union Payments API
  slug: western-union-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/western-union/refs/heads/main/openapi/western-union-payments-api-openapi.yml
- filename: western-union-quotes-api-openapi.yml
  format: yaml
  label: western-union Quotes API
  slug: western-union-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/western-union/refs/heads/main/openapi/western-union-quotes-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: westernunion.com
  spf: true
hosts:
- cert_expires: Oct 28 23:59:59 2026 GMT
  host: www.westernunion.com
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 21 23:59:59 2026 GMT
  host: developer.westernunion.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: api.westernunion.com
  https: false
kind: domain-security
layout: security
method: probed
name: Western Union Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for western-union, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: western-union
provider_slug: western-union
slug: western-union-domain-security
source_filename: western-union-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.westernunion.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 86400\n- host: developer.westernunion.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 23:59:59 2026 GMT\n  hsts: null\n- host: api.westernunion.com\n  https: false\ndomains:\n- domain: westernunion.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/western-union/refs/heads/main/security/western-union-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fortune 500
---
