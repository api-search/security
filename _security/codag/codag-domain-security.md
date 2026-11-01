---
api_specs:
- filename: codag-activate-api-openapi.yml
  format: yaml
  label: Codag Activate API
  slug: codag-activate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codag/openapi/codag-activate-api-openapi.yml
- filename: codag-admin-api-openapi.yml
  format: yaml
  label: Codag Admin API
  slug: codag-admin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codag/openapi/codag-admin-api-openapi.yml
- filename: codag-anonymous-api-openapi.yml
  format: yaml
  label: Codag Anonymous API
  slug: codag-anonymous-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codag/openapi/codag-anonymous-api-openapi.yml
- filename: codag-auth-api-openapi.yml
  format: yaml
  label: Codag Auth API
  slug: codag-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codag/openapi/codag-auth-api-openapi.yml
- filename: codag-billing-api-openapi.yml
  format: yaml
  label: Codag Billing API
  slug: codag-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codag/openapi/codag-billing-api-openapi.yml
- filename: codag-capsule-api-openapi.yml
  format: yaml
  label: Codag Capsule API
  slug: codag-capsule-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codag/openapi/codag-capsule-api-openapi.yml
- filename: codag-cli-api-openapi.yml
  format: yaml
  label: Codag Cli API
  slug: codag-cli-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codag/openapi/codag-cli-api-openapi.yml
- filename: codag-compact-api-openapi.yml
  format: yaml
  label: Codag Compact API
  slug: codag-compact-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codag/openapi/codag-compact-api-openapi.yml
- filename: codag-free-api-openapi.yml
  format: yaml
  label: Codag Free API
  slug: codag-free-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codag/openapi/codag-free-api-openapi.yml
- filename: codag-health-api-openapi.yml
  format: yaml
  label: Codag Health API
  slug: codag-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codag/openapi/codag-health-api-openapi.yml
- filename: codag-incident-memory-api-openapi.yml
  format: yaml
  label: Codag Incident Memory API
  slug: codag-incident-memory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codag/openapi/codag-incident-memory-api-openapi.yml
- filename: codag-install-sh-api-openapi.yml
  format: yaml
  label: Codag Install.sh API
  slug: codag-install-sh-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codag/openapi/codag-install-sh-api-openapi.yml
- filename: codag-internal-api-openapi.yml
  format: yaml
  label: Codag Internal API
  slug: codag-internal-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codag/openapi/codag-internal-api-openapi.yml
- filename: codag-onboard-api-openapi.yml
  format: yaml
  label: Codag Onboard API
  slug: codag-onboard-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codag/openapi/codag-onboard-api-openapi.yml
- filename: codag-org-api-openapi.yml
  format: yaml
  label: Codag Org API
  slug: codag-org-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codag/openapi/codag-org-api-openapi.yml
- filename: codag-orgs-api-openapi.yml
  format: yaml
  label: Codag Orgs API
  slug: codag-orgs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codag/openapi/codag-orgs-api-openapi.yml
- filename: codag-parse-api-openapi.yml
  format: yaml
  label: Codag Parse API
  slug: codag-parse-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codag/openapi/codag-parse-api-openapi.yml
- filename: codag-whoami-api-openapi.yml
  format: yaml
  label: Codag Whoami API
  slug: codag-whoami-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codag/openapi/codag-whoami-api-openapi.yml
- filename: codag-oauth-api-openapi.yml
  format: yaml
  label: Codag OAUTH API
  slug: codag-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codag/openapi/codag-oauth-api-openapi.yml
- filename: codag-agent-cost-api-openapi.yml
  format: yaml
  label: Codag Agent Cost API
  slug: codag-agent-cost-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codag/openapi/codag-agent-cost-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: codag.ai
  spf: true
hosts:
- cert_expires: Sep 12 02:23:37 2026 GMT
  host: codag.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 03:08:04 2026 GMT
  host: api.codag.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Codag Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Codag, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Codag
provider_slug: codag
slug: codag-domain-security
source_filename: codag-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: codag.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 02:23:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.codag.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 03:08:04 2026 GMT\n  hsts: null\ndomains:\n- domain: codag.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/codag/security/codag-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Developer Tools
- Logging
- Observability
- Log Compression
- AI Agents
- MCP
- LLM Tooling
- Debugging
- Y Combinator
---
