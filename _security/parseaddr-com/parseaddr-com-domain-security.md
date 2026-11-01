---
api_specs:
- filename: parseaddr-com-checkout-api-openapi.yml
  format: yaml
  label: parseaddr-com Checkout API
  slug: parseaddr-com-checkout-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/parseaddr-com/openapi/parseaddr-com-checkout-api-openapi.yml
- filename: parseaddr-com-credits-api-openapi.yml
  format: yaml
  label: parseaddr-com Credits API
  slug: parseaddr-com-credits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/parseaddr-com/openapi/parseaddr-com-credits-api-openapi.yml
- filename: parseaddr-com-expand-api-openapi.yml
  format: yaml
  label: parseaddr-com Expand API
  slug: parseaddr-com-expand-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/parseaddr-com/openapi/parseaddr-com-expand-api-openapi.yml
- filename: parseaddr-com-health-api-openapi.yml
  format: yaml
  label: parseaddr-com Health API
  slug: parseaddr-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/parseaddr-com/openapi/parseaddr-com-health-api-openapi.yml
- filename: parseaddr-com-parse-api-openapi.yml
  format: yaml
  label: parseaddr-com Parse API
  slug: parseaddr-com-parse-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/parseaddr-com/openapi/parseaddr-com-parse-api-openapi.yml
- filename: parseaddr-com-signup-api-openapi.yml
  format: yaml
  label: parseaddr-com Signup API
  slug: parseaddr-com-signup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/parseaddr-com/openapi/parseaddr-com-signup-api-openapi.yml
- filename: parseaddr-com-usage-api-openapi.yml
  format: yaml
  label: parseaddr-com Usage API
  slug: parseaddr-com-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/parseaddr-com/openapi/parseaddr-com-usage-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: parseaddr.com
  spf: false
hosts:
- cert_expires: Dec 28 20:56:05 2026 GMT
  host: parseaddr.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Parseaddr Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for parseaddr-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: parseaddr-com
provider_slug: parseaddr-com
slug: parseaddr-com-domain-security
source_filename: parseaddr-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: parseaddr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 28 20:56:05 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: parseaddr.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/parseaddr-com/security/parseaddr-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Address
- Parsing
- API
- libpostal
---
