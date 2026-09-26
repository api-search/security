---
api_specs:
- filename: keploy-api-keys-api-openapi.yml
  format: yaml
  label: Keploy API Keys API
  slug: keploy-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keploy/refs/heads/main/openapi/keploy-api-keys-api-openapi.yml
- filename: keploy-apps-api-openapi.yml
  format: yaml
  label: Keploy Apps API
  slug: keploy-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keploy/refs/heads/main/openapi/keploy-apps-api-openapi.yml
- filename: keploy-branches-api-openapi.yml
  format: yaml
  label: Keploy Branches API
  slug: keploy-branches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keploy/refs/heads/main/openapi/keploy-branches-api-openapi.yml
- filename: keploy-clusters-api-openapi.yml
  format: yaml
  label: Keploy Clusters API
  slug: keploy-clusters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keploy/refs/heads/main/openapi/keploy-clusters-api-openapi.yml
- filename: keploy-company-api-openapi.yml
  format: yaml
  label: Keploy Company API
  slug: keploy-company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keploy/refs/heads/main/openapi/keploy-company-api-openapi.yml
- filename: keploy-generation-history-api-openapi.yml
  format: yaml
  label: Keploy Generation History API
  slug: keploy-generation-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keploy/refs/heads/main/openapi/keploy-generation-history-api-openapi.yml
- filename: keploy-jobs-api-openapi.yml
  format: yaml
  label: Keploy Jobs API
  slug: keploy-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keploy/refs/heads/main/openapi/keploy-jobs-api-openapi.yml
- filename: keploy-load-tests-api-openapi.yml
  format: yaml
  label: Keploy Load Tests API
  slug: keploy-load-tests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keploy/refs/heads/main/openapi/keploy-load-tests-api-openapi.yml
- filename: keploy-recordings-api-openapi.yml
  format: yaml
  label: Keploy Recordings API
  slug: keploy-recordings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keploy/refs/heads/main/openapi/keploy-recordings-api-openapi.yml
- filename: keploy-smartset-api-openapi.yml
  format: yaml
  label: Keploy Smart Set API
  slug: keploy-smartset-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keploy/refs/heads/main/openapi/keploy-smartset-api-openapi.yml
- filename: keploy-test-reports-api-openapi.yml
  format: yaml
  label: Keploy Test Reports API
  slug: keploy-test-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keploy/refs/heads/main/openapi/keploy-test-reports-api-openapi.yml
- filename: keploy-test-runs-api-openapi.yml
  format: yaml
  label: Keploy Test Runs API
  slug: keploy-test-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keploy/refs/heads/main/openapi/keploy-test-runs-api-openapi.yml
- filename: keploy-test-suites-api-openapi.yml
  format: yaml
  label: Keploy Test Suites API
  slug: keploy-test-suites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keploy/refs/heads/main/openapi/keploy-test-suites-api-openapi.yml
- filename: keploy-users-api-openapi.yml
  format: yaml
  label: Keploy Users API
  slug: keploy-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keploy/refs/heads/main/openapi/keploy-users-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: keploy.io
  spf: true
hosts:
- cert_expires: Nov  1 23:59:59 2026 GMT
  host: keploy.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 02:28:07 2026 GMT
  host: api.keploy.io
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Keploy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Keploy, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Keploy
provider_slug: keploy
slug: keploy-domain-security
source_filename: keploy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: keploy.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.keploy.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 02:28:07 2026 GMT\n  hsts: null\ndomains:\n- domain: keploy.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/keploy/refs/heads/main/security/keploy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Testing & QA
- API Testing
- Integration/Regression Testing
- Unit Test Generation
- Contract Testing
- CI/CD
- Developer Tools
- AI / Agent Tooling
- eBPF / Observability
- Test Data & Mocking
- Testing
---
