---
api_specs:
- filename: scorecard-metrics-api-openapi.yml
  format: yaml
  label: Scorecard Metrics API
  slug: scorecard-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scorecard/refs/heads/main/openapi/scorecard-metrics-api-openapi.yml
- filename: scorecard-projects-api-openapi.yml
  format: yaml
  label: Scorecard Projects API
  slug: scorecard-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scorecard/refs/heads/main/openapi/scorecard-projects-api-openapi.yml
- filename: scorecard-records-api-openapi.yml
  format: yaml
  label: Scorecard Records API
  slug: scorecard-records-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scorecard/refs/heads/main/openapi/scorecard-records-api-openapi.yml
- filename: scorecard-runs-api-openapi.yml
  format: yaml
  label: Scorecard Runs API
  slug: scorecard-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scorecard/refs/heads/main/openapi/scorecard-runs-api-openapi.yml
- filename: scorecard-systems-api-openapi.yml
  format: yaml
  label: Scorecard Systems API
  slug: scorecard-systems-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scorecard/refs/heads/main/openapi/scorecard-systems-api-openapi.yml
- filename: scorecard-testcases-api-openapi.yml
  format: yaml
  label: Scorecard Testcases API
  slug: scorecard-testcases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scorecard/refs/heads/main/openapi/scorecard-testcases-api-openapi.yml
- filename: scorecard-testsets-api-openapi.yml
  format: yaml
  label: Scorecard Testsets API
  slug: scorecard-testsets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scorecard/refs/heads/main/openapi/scorecard-testsets-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: scorecard.io
  spf: true
hosts:
- cert_expires: Sep 22 00:39:17 2026 GMT
  host: www.scorecard.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 04:10:14 2026 GMT
  host: docs.scorecard.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 16:30:58 2026 GMT
  host: api2.scorecard.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Scorecard Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Scorecard, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Scorecard
provider_slug: scorecard
slug: scorecard-domain-security
source_filename: scorecard-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.scorecard.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 00:39:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.scorecard.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 04:10:14 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api2.scorecard.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 16:30:58 2026 GMT\n  hsts: null\ndomains:\n- domain: scorecard.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scorecard/refs/heads/main/security/scorecard-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Agents
- Evaluation
- Testing
- LLM
- Observability
- Simulation
- Developer Tools
- MCP
---
