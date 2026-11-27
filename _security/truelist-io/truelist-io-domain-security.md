---
api_specs:
- filename: truelist-io-batch-email-validation-api-openapi.yml
  format: yaml
  label: Truelist Batch email validation API
  slug: truelist-io-batch-email-validation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/truelist-io/openapi/truelist-io-batch-email-validation-api-openapi.yml
- filename: truelist-io-me-api-openapi.yml
  format: yaml
  label: Truelist Me API
  slug: truelist-io-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/truelist-io/openapi/truelist-io-me-api-openapi.yml
- filename: truelist-io-retrieving-results-api-openapi.yml
  format: yaml
  label: Truelist Retrieving results API
  slug: truelist-io-retrieving-results-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/truelist-io/openapi/truelist-io-retrieving-results-api-openapi.yml
- filename: truelist-io-single-email-validation-api-openapi.yml
  format: yaml
  label: Truelist Single email validation API
  slug: truelist-io-single-email-validation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/truelist-io/openapi/truelist-io-single-email-validation-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dns_aid:
    checked: '2026-11-27'
    published: false
  dnssec: false
  domain: truelist.io
  spf: true
hosts:
- cert_expires: Feb 21 12:30:05 2027 GMT
  host: truelist.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Truelist Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Truelist, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Truelist
provider_slug: truelist-io
slug: truelist-io-domain-security
source_filename: truelist-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: truelist.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 21 12:30:05 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: truelist.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n  dns_aid:\n    checked: '2026-11-27'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/truelist-io/security/truelist-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Email Validation
- API
- SaaS
- Data Quality
- Marketing
---
