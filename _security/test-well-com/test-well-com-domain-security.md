---
api_specs:
- filename: test-well-com-catalog-api-openapi.yml
  format: yaml
  label: TestWell Catalog API
  slug: test-well-com-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/test-well-com/openapi/test-well-com-catalog-api-openapi.yml
- filename: test-well-com-catalog-json-api-openapi.yml
  format: yaml
  label: TestWell Catalog.json API
  slug: test-well-com-catalog-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/test-well-com/openapi/test-well-com-catalog-json-api-openapi.yml
- filename: test-well-com-checkout-api-openapi.yml
  format: yaml
  label: TestWell Checkout API
  slug: test-well-com-checkout-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/test-well-com/openapi/test-well-com-checkout-api-openapi.yml
- filename: test-well-com-compare-api-openapi.yml
  format: yaml
  label: TestWell Compare API
  slug: test-well-com-compare-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/test-well-com/openapi/test-well-com-compare-api-openapi.yml
- filename: test-well-com-content-api-openapi.yml
  format: yaml
  label: TestWell Content API
  slug: test-well-com-content-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/test-well-com/openapi/test-well-com-content-api-openapi.yml
- filename: test-well-com-locations-api-openapi.yml
  format: yaml
  label: TestWell Locations API
  slug: test-well-com-locations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/test-well-com/openapi/test-well-com-locations-api-openapi.yml
- filename: test-well-com-quote-api-openapi.yml
  format: yaml
  label: TestWell Quote API
  slug: test-well-com-quote-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/test-well-com/openapi/test-well-com-quote-api-openapi.yml
- filename: test-well-com-reference-api-openapi.yml
  format: yaml
  label: TestWell Reference API
  slug: test-well-com-reference-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/test-well-com/openapi/test-well-com-reference-api-openapi.yml
- filename: test-well-com-reference-ranges-json-api-openapi.yml
  format: yaml
  label: TestWell Reference Ranges.json API
  slug: test-well-com-reference-ranges-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/test-well-com/openapi/test-well-com-reference-ranges-json-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dns_aid:
    checked: '2026-11-26'
    published: false
  dnssec: false
  domain: test-well.com
  spf: true
hosts:
- cert_expires: Jan 27 06:41:14 2027 GMT
  host: test-well.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: TestWell Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TestWell, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: TestWell
provider_slug: test-well-com
slug: test-well-com-domain-security
source_filename: test-well-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: test-well.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 06:41:14 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: test-well.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n  dns_aid:\n    checked: '2026-11-26'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/test-well-com/security/test-well-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Medical
- Direct-to-Consumer
- LabTesting
- Healthcare
- US
---
