---
api_specs:
- filename: vatstack-batches-api-openapi.yml
  format: yaml
  label: Vatstack Batches API
  slug: vatstack-batches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vatstack/refs/heads/main/openapi/vatstack-batches-api-openapi.yml
- filename: vatstack-evidences-api-openapi.yml
  format: yaml
  label: Vatstack Evidences API
  slug: vatstack-evidences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vatstack/refs/heads/main/openapi/vatstack-evidences-api-openapi.yml
- filename: vatstack-hits-api-openapi.yml
  format: yaml
  label: Vatstack Hits API
  slug: vatstack-hits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vatstack/refs/heads/main/openapi/vatstack-hits-api-openapi.yml
- filename: vatstack-quotes-api-openapi.yml
  format: yaml
  label: Vatstack Quotes API
  slug: vatstack-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vatstack/refs/heads/main/openapi/vatstack-quotes-api-openapi.yml
- filename: vatstack-rates-api-openapi.yml
  format: yaml
  label: Vatstack Rates API
  slug: vatstack-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vatstack/refs/heads/main/openapi/vatstack-rates-api-openapi.yml
- filename: vatstack-supplies-api-openapi.yml
  format: yaml
  label: Vatstack Supplies API
  slug: vatstack-supplies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vatstack/refs/heads/main/openapi/vatstack-supplies-api-openapi.yml
- filename: vatstack-validations-api-openapi.yml
  format: yaml
  label: Vatstack Validations API
  slug: vatstack-validations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vatstack/refs/heads/main/openapi/vatstack-validations-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: vatstack.com
  spf: true
hosts:
- cert_expires: Sep 16 05:46:51 2026 GMT
  host: vatstack.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 18:17:02 2026 GMT
  host: api.vatstack.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vatstack Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vatstack, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Vatstack
provider_slug: vatstack
slug: vatstack-domain-security
source_filename: vatstack-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vatstack.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 05:46:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.vatstack.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 18:17:02 2026 GMT\n  hsts: null\ndomains:\n- domain: vatstack.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vatstack/refs/heads/main/security/vatstack-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- VAT
- Tax
- Validation
- EU
- Europe
- Compliance
- Finance
- Business
---
