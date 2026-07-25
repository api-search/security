---
api_specs:
- filename: duck-creek-billing-api-openapi.yml
  format: yaml
  label: Duck Creek Billing API
  slug: duck-creek-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/duck-creek/refs/heads/main/openapi/duck-creek-billing-api-openapi.yml
- filename: duck-creek-claims-api-openapi.yml
  format: yaml
  label: Duck Creek Claims API
  slug: duck-creek-claims-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/duck-creek/refs/heads/main/openapi/duck-creek-claims-api-openapi.yml
- filename: duck-creek-billing-api-openapi.yml
  format: yaml
  label: duck-creek Billing API
  slug: duck-creek-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/duck-creek/refs/heads/main/openapi/duck-creek-billing-api-openapi.yml
- filename: duck-creek-claims-api-openapi.yml
  format: yaml
  label: duck-creek Claims API
  slug: duck-creek-claims-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/duck-creek/refs/heads/main/openapi/duck-creek-claims-api-openapi.yml
- filename: duck-creek-policies-api-openapi.yml
  format: yaml
  label: duck-creek Policies API
  slug: duck-creek-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/duck-creek/refs/heads/main/openapi/duck-creek-policies-api-openapi.yml
- filename: duck-creek-products-api-openapi.yml
  format: yaml
  label: duck-creek Products API
  slug: duck-creek-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/duck-creek/refs/heads/main/openapi/duck-creek-products-api-openapi.yml
- filename: duck-creek-quotes-api-openapi.yml
  format: yaml
  label: duck-creek Quotes API
  slug: duck-creek-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/duck-creek/refs/heads/main/openapi/duck-creek-quotes-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: duckcreek.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: duckcreek.dev
  spf: false
hosts:
- cert_expires: Oct  2 09:02:03 2026 GMT
  host: www.duckcreek.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- host: duckcreek.dev
  https: false
- host: api.duckcreek.com
  https: false
kind: domain-security
layout: security
method: probed
name: Duck Creek Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for duck-creek, probed live across 3 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: duck-creek
provider_slug: duck-creek
slug: duck-creek-domain-security
source_filename: duck-creek-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.duckcreek.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 09:02:03 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: duckcreek.dev\n  https: false\n- host: api.duckcreek.com\n  https: false\ndomains:\n- domain: duckcreek.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: duckcreek.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/duck-creek/refs/heads/main/security/duck-creek-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags: []
---
