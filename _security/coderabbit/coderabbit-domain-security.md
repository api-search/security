---
api_specs:
- filename: coderabbit-audit-logs-api-openapi.yml
  format: yaml
  label: CodeRabbit Audit Logs API
  slug: coderabbit-audit-logs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coderabbit/openapi/coderabbit-audit-logs-api-openapi.yml
- filename: coderabbit-learnings-api-openapi.yml
  format: yaml
  label: CodeRabbit Learnings API
  slug: coderabbit-learnings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coderabbit/openapi/coderabbit-learnings-api-openapi.yml
- filename: coderabbit-metrics-api-openapi.yml
  format: yaml
  label: CodeRabbit Metrics API
  slug: coderabbit-metrics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coderabbit/openapi/coderabbit-metrics-api-openapi.yml
- filename: coderabbit-organizations-api-openapi.yml
  format: yaml
  label: CodeRabbit Organizations API
  slug: coderabbit-organizations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coderabbit/openapi/coderabbit-organizations-api-openapi.yml
- filename: coderabbit-report-generate-api-openapi.yml
  format: yaml
  label: CodeRabbit Report.generate API
  slug: coderabbit-report-generate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coderabbit/openapi/coderabbit-report-generate-api-openapi.yml
- filename: coderabbit-role-management-api-openapi.yml
  format: yaml
  label: CodeRabbit Role Management API
  slug: coderabbit-role-management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coderabbit/openapi/coderabbit-role-management-api-openapi.yml
- filename: coderabbit-security-api-openapi.yml
  format: yaml
  label: CodeRabbit Security API
  slug: coderabbit-security-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coderabbit/openapi/coderabbit-security-api-openapi.yml
- filename: coderabbit-users-api-openapi.yml
  format: yaml
  label: CodeRabbit Users API
  slug: coderabbit-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coderabbit/openapi/coderabbit-users-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: coderabbit.ai
  spf: true
hosts:
- cert_expires: Oct  4 02:03:50 2026 GMT
  host: www.coderabbit.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 12:48:56 2026 GMT
  host: docs.coderabbit.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 17:10:07 2026 GMT
  host: api.coderabbit.ai
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Coderabbit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CodeRabbit, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: CodeRabbit
provider_slug: coderabbit
slug: coderabbit-domain-security
source_filename: coderabbit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.coderabbit.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 02:03:50 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.coderabbit.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 12:48:56 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.coderabbit.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 17:10:07 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: coderabbit.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/coderabbit/security/coderabbit-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Code Review
- Developer Tools
- Pull Requests
- DevOps
---
