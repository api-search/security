---
api_specs:
- filename: wiremock-near-misses-api-openapi.yml
  format: yaml
  label: WireMock Near Misses API
  slug: wiremock-near-misses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wiremock/refs/heads/main/openapi/wiremock-near-misses-api-openapi.yml
- filename: wiremock-recordings-api-openapi.yml
  format: yaml
  label: WireMock Recordings API
  slug: wiremock-recordings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wiremock/refs/heads/main/openapi/wiremock-recordings-api-openapi.yml
- filename: wiremock-requests-api-openapi.yml
  format: yaml
  label: WireMock Requests API
  slug: wiremock-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wiremock/refs/heads/main/openapi/wiremock-requests-api-openapi.yml
- filename: wiremock-scenarios-api-openapi.yml
  format: yaml
  label: WireMock Scenarios API
  slug: wiremock-scenarios-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wiremock/refs/heads/main/openapi/wiremock-scenarios-api-openapi.yml
- filename: wiremock-stub-mappings-api-openapi.yml
  format: yaml
  label: WireMock Stub Mappings API
  slug: wiremock-stub-mappings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wiremock/refs/heads/main/openapi/wiremock-stub-mappings-api-openapi.yml
- filename: wiremock-system-api-openapi.yml
  format: yaml
  label: WireMock System API
  slug: wiremock-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wiremock/refs/heads/main/openapi/wiremock-system-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: wiremock.org
  spf: false
hosts:
- cert_expires: Nov 11 23:59:59 2026 GMT
  host: wiremock.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wiremock Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for WireMock, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: WireMock
provider_slug: wiremock
slug: wiremock-domain-security
source_filename: wiremock-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wiremock.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 11 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: wiremock.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wiremock/refs/heads/main/security/wiremock-domain-security.yml
summary_line: TLSv1.3
tags:
- API Mocking
- Mock Server
- Mocking
- Platform
- Stubs
- Testing
---
