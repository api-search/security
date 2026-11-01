---
api_specs:
- filename: decide-fyi-action-execution-api-openapi.yml
  format: yaml
  label: decide-fyi Action Execution API
  slug: decide-fyi-action-execution-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/decide-fyi/openapi/decide-fyi-action-execution-api-openapi.yml
- filename: decide-fyi-anomalies-api-openapi.yml
  format: yaml
  label: decide-fyi Anomalies API
  slug: decide-fyi-anomalies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/decide-fyi/openapi/decide-fyi-anomalies-api-openapi.yml
- filename: decide-fyi-audit-chain-api-openapi.yml
  format: yaml
  label: decide-fyi Audit Chain API
  slug: decide-fyi-audit-chain-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/decide-fyi/openapi/decide-fyi-audit-chain-api-openapi.yml
- filename: decide-fyi-benchmarks-api-openapi.yml
  format: yaml
  label: decide-fyi Benchmarks API
  slug: decide-fyi-benchmarks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/decide-fyi/openapi/decide-fyi-benchmarks-api-openapi.yml
- filename: decide-fyi-confidence-api-openapi.yml
  format: yaml
  label: decide-fyi Confidence API
  slug: decide-fyi-confidence-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/decide-fyi/openapi/decide-fyi-confidence-api-openapi.yml
- filename: decide-fyi-counterfactuals-api-openapi.yml
  format: yaml
  label: decide-fyi Counterfactuals API
  slug: decide-fyi-counterfactuals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/decide-fyi/openapi/decide-fyi-counterfactuals-api-openapi.yml
- filename: decide-fyi-crm-sync-api-openapi.yml
  format: yaml
  label: decide-fyi CRM Sync API
  slug: decide-fyi-crm-sync-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/decide-fyi/openapi/decide-fyi-crm-sync-api-openapi.yml
- filename: decide-fyi-decision-packets-api-openapi.yml
  format: yaml
  label: decide-fyi Decision Packets API
  slug: decide-fyi-decision-packets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/decide-fyi/openapi/decide-fyi-decision-packets-api-openapi.yml
- filename: decide-fyi-decision-protocol-api-openapi.yml
  format: yaml
  label: decide-fyi Decision Protocol API
  slug: decide-fyi-decision-protocol-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/decide-fyi/openapi/decide-fyi-decision-protocol-api-openapi.yml
- filename: decide-fyi-effectiveness-api-openapi.yml
  format: yaml
  label: decide-fyi Effectiveness API
  slug: decide-fyi-effectiveness-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/decide-fyi/openapi/decide-fyi-effectiveness-api-openapi.yml
- filename: decide-fyi-outcome-tracking-api-openapi.yml
  format: yaml
  label: decide-fyi Outcome Tracking API
  slug: decide-fyi-outcome-tracking-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/decide-fyi/openapi/decide-fyi-outcome-tracking-api-openapi.yml
- filename: decide-fyi-policy-patterns-api-openapi.yml
  format: yaml
  label: decide-fyi Policy Patterns API
  slug: decide-fyi-policy-patterns-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/decide-fyi/openapi/decide-fyi-policy-patterns-api-openapi.yml
- filename: decide-fyi-registries-api-openapi.yml
  format: yaml
  label: decide-fyi Registries API
  slug: decide-fyi-registries-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/decide-fyi/openapi/decide-fyi-registries-api-openapi.yml
- filename: decide-fyi-verification-api-openapi.yml
  format: yaml
  label: decide-fyi Verification API
  slug: decide-fyi-verification-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/decide-fyi/openapi/decide-fyi-verification-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: decide.fyi
  spf: true
hosts:
- cert_expires: Dec  1 08:08:08 2026 GMT
  host: decide.fyi
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Decide Fyi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for decide-fyi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: decide-fyi
provider_slug: decide-fyi
slug: decide-fyi-domain-security
source_filename: decide-fyi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: decide.fyi\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 08:08:08 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: decide.fyi\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/decide-fyi/security/decide-fyi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Decision API
- Rule Engine
- SaaS
- Automation
- Runtime
---
