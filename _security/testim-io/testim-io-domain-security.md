---
api_specs:
- filename: testim-io-branches-api-openapi.yml
  format: yaml
  label: Testim Io Branches API
  slug: testim-io-branches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/testim-io/refs/heads/main/openapi/testim-io-branches-api-openapi.yml
- filename: testim-io-executions-api-openapi.yml
  format: yaml
  label: Testim Io Executions API
  slug: testim-io-executions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/testim-io/refs/heads/main/openapi/testim-io-executions-api-openapi.yml
- filename: testim-io-labels-api-openapi.yml
  format: yaml
  label: Testim Io Labels API
  slug: testim-io-labels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/testim-io/refs/heads/main/openapi/testim-io-labels-api-openapi.yml
- filename: testim-io-mobile-applications-api-openapi.yml
  format: yaml
  label: Testim Io Mobile Applications API
  slug: testim-io-mobile-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/testim-io/refs/heads/main/openapi/testim-io-mobile-applications-api-openapi.yml
- filename: testim-io-suites-api-openapi.yml
  format: yaml
  label: Testim Io Suites API
  slug: testim-io-suites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/testim-io/refs/heads/main/openapi/testim-io-suites-api-openapi.yml
- filename: testim-io-test-plans-api-openapi.yml
  format: yaml
  label: Testim Io Test plans API
  slug: testim-io-test-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/testim-io/refs/heads/main/openapi/testim-io-test-plans-api-openapi.yml
- filename: testim-io-tests-api-openapi.yml
  format: yaml
  label: Testim Io Tests API
  slug: testim-io-tests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/testim-io/refs/heads/main/openapi/testim-io-tests-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: testim.io
  spf: true
hosts:
- cert_expires: Mar  2 23:59:59 2027 GMT
  host: api.testim.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 23:59:59 2026 GMT
  host: api.eu.testim.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Testim Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Testim Io, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Testim Io
provider_slug: testim-io
slug: testim-io-domain-security
source_filename: testim-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.testim.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  2 23:59:59 2027 GMT\n  hsts: null\n- host: api.eu.testim.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: testim.io\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/testim-io/refs/heads/main/security/testim-io-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- API Testing
- Test Automation
- Quality Assurance
- CI/CD
- Mobile Testing
- Software Testing
- DevOps
- Company
---
