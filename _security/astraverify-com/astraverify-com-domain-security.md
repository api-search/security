---
api_specs:
- filename: astraverify-com-discoverability-api-openapi.yml
  format: yaml
  label: AstraVerify Discoverability API
  slug: astraverify-com-discoverability-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/astraverify-com/openapi/astraverify-com-discoverability-api-openapi.yml
- filename: astraverify-com-email-api-openapi.yml
  format: yaml
  label: AstraVerify Email API
  slug: astraverify-com-email-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/astraverify-com/openapi/astraverify-com-email-api-openapi.yml
- filename: astraverify-com-fetch-as-api-openapi.yml
  format: yaml
  label: AstraVerify Fetch As API
  slug: astraverify-com-fetch-as-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/astraverify-com/openapi/astraverify-com-fetch-as-api-openapi.yml
- filename: astraverify-com-report-api-openapi.yml
  format: yaml
  label: AstraVerify Report API
  slug: astraverify-com-report-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/astraverify-com/openapi/astraverify-com-report-api-openapi.yml
- filename: astraverify-com-verify-api-openapi.yml
  format: yaml
  label: AstraVerify Verify API
  slug: astraverify-com-verify-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/astraverify-com/openapi/astraverify-com-verify-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: astraverify.com
  spf: true
hosts:
- cert_expires: Dec 16 05:33:33 2026 GMT
  host: astraverify.com
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: AstraVerify Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AstraVerify, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: AstraVerify
provider_slug: astraverify-com
slug: astraverify-com-domain-security
source_filename: astraverify-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: astraverify.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 05:33:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: astraverify.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/astraverify-com/security/astraverify-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Security
- Email
- Artificial Intelligence
- Discoverability
- Domain
---
