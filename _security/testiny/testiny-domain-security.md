---
api_specs:
- filename: testiny-openapi.yml
  format: yaml
  label: Testiny Test Runs API
  slug: testiny-test-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/testiny/refs/heads/main/openapi/testiny-openapi.yml
- filename: testiny-openapi.yml
  format: yaml
  label: Testiny Test Cases API
  slug: testiny-test-cases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/testiny/refs/heads/main/openapi/testiny-openapi.yml
- filename: testiny-openapi.yml
  format: yaml
  label: Testiny Test Plans API
  slug: testiny-test-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/testiny/refs/heads/main/openapi/testiny-openapi.yml
- filename: testiny-openapi.yml
  format: yaml
  label: Testiny Projects API
  slug: testiny-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/testiny/refs/heads/main/openapi/testiny-openapi.yml
- filename: testiny-openapi.yml
  format: yaml
  label: Testiny Automation API
  slug: testiny-automation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/testiny/refs/heads/main/openapi/testiny-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_pct: 80
  dmarc_policy: quarantine
  dnssec: false
  domain: testiny.io
  spf: true
  spf_policy: ~all
hosts:
- cert_expires: Sep 15 12:24:54 2026 GMT
  host: www.testiny.io
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 09:29:54 2026 GMT
  host: app.testiny.io
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: testiny.io
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  http_status: 308
  https: true
kind: domain-security
layout: security
method: probed
name: Testiny Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Testiny, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Testiny
provider_slug: testiny
slug: testiny-domain-security
source_filename: testiny-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.testiny.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 12:24:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n- host: app.testiny.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 09:29:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n- host: testiny.io\n  https: true\n  http_status: 308\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\ndomains:\n- domain: testiny.io\n  dnssec: false\n  caa: []\n  spf: true\n  spf_policy: ~all\n  dmarc: true\n  dmarc_policy: quarantine\n  dmarc_pct: 80\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/testiny/refs/heads/main/security/testiny-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Test Runs
- Test Management
- QA
- Test Cases
- Test Automation
- Quality Assurance
- Testing
---
