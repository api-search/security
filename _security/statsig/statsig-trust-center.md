---
api_specs:
- filename: statsig-events-api-openapi.yml
  format: yaml
  label: Statsig Events API
  slug: events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/statsig/refs/heads/main/openapi/statsig-events-api-openapi.yml
- filename: statsig-audit-logs-api-openapi.yml
  format: yaml
  label: statsig Audit Logs API
  slug: statsig-audit-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/statsig/refs/heads/main/openapi/statsig-audit-logs-api-openapi.yml
- filename: statsig-autotunes-api-openapi.yml
  format: yaml
  label: statsig Autotunes API
  slug: statsig-autotunes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/statsig/refs/heads/main/openapi/statsig-autotunes-api-openapi.yml
- filename: statsig-configuration-api-openapi.yml
  format: yaml
  label: statsig Configuration API
  slug: statsig-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/statsig/refs/heads/main/openapi/statsig-configuration-api-openapi.yml
- filename: statsig-dynamic-configs-api-openapi.yml
  format: yaml
  label: statsig Dynamic Configs API
  slug: statsig-dynamic-configs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/statsig/refs/heads/main/openapi/statsig-dynamic-configs-api-openapi.yml
- filename: statsig-experiments-api-openapi.yml
  format: yaml
  label: statsig Experiments API
  slug: statsig-experiments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/statsig/refs/heads/main/openapi/statsig-experiments-api-openapi.yml
- filename: statsig-feature-gates-api-openapi.yml
  format: yaml
  label: statsig Feature Gates API
  slug: statsig-feature-gates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/statsig/refs/heads/main/openapi/statsig-feature-gates-api-openapi.yml
- filename: statsig-gates-api-openapi.yml
  format: yaml
  label: statsig Gates API
  slug: statsig-gates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/statsig/refs/heads/main/openapi/statsig-gates-api-openapi.yml
- filename: statsig-holdouts-api-openapi.yml
  format: yaml
  label: statsig Holdouts API
  slug: statsig-holdouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/statsig/refs/heads/main/openapi/statsig-holdouts-api-openapi.yml
- filename: statsig-initialization-api-openapi.yml
  format: yaml
  label: statsig Initialization API
  slug: statsig-initialization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/statsig/refs/heads/main/openapi/statsig-initialization-api-openapi.yml
- filename: statsig-keys-api-openapi.yml
  format: yaml
  label: statsig Keys API
  slug: statsig-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/statsig/refs/heads/main/openapi/statsig-keys-api-openapi.yml
- filename: statsig-layers-api-openapi.yml
  format: yaml
  label: statsig Layers API
  slug: statsig-layers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/statsig/refs/heads/main/openapi/statsig-layers-api-openapi.yml
- filename: statsig-metrics-api-openapi.yml
  format: yaml
  label: statsig Metrics API
  slug: statsig-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/statsig/refs/heads/main/openapi/statsig-metrics-api-openapi.yml
- filename: statsig-segments-api-openapi.yml
  format: yaml
  label: statsig Segments API
  slug: statsig-segments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/statsig/refs/heads/main/openapi/statsig-segments-api-openapi.yml
- filename: statsig-tags-api-openapi.yml
  format: yaml
  label: statsig Tags API
  slug: statsig-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/statsig/refs/heads/main/openapi/statsig-tags-api-openapi.yml
- filename: statsig-target-apps-api-openapi.yml
  format: yaml
  label: statsig Target Apps API
  slug: statsig-target-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/statsig/refs/heads/main/openapi/statsig-target-apps-api-openapi.yml
- filename: statsig-users-api-openapi.yml
  format: yaml
  label: statsig Users API
  slug: statsig-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/statsig/refs/heads/main/openapi/statsig-users-api-openapi.yml
- filename: statsig-console-api-openapi.json
  format: json
  label: statsig Console API
  slug: statsig-console-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/statsig/refs/heads/main/openapi/statsig-console-api-openapi.json
certification_count: 4
certifications:
- SOC 2 Type II
- ISO 27001
- GDPR
- HIPAA
description: ''
kind: trust-center
layout: security
name: Statsig Trust Center
name_suffix: Trust Center
overview: Statsig maintains a public trust center documenting SOC 2 Type II, ISO 27001, GDPR, and HIPAA compliance.
provider_name: Statsig
provider_slug: statsig
slug: statsig-trust-center
source_filename: statsig-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: searched\nprobe: true\nsource: https://trust.statsig.com/\nurl: https://trust.statsig.com/\nresolved_url: https://trust.amplitude.com/?product_id=25a85de2-f369-4ee0-bd69-5fb5912f39ae\ndomain_note: >-\n  The trust center is reached at Statsig's own subdomain, trust.statsig.com, which HTTP-redirects\n  to trust.amplitude.com scoped to a Statsig product_id. The cross-domain hop is justified by the\n  provider's own surface in two independent places: Statsig itself points trust.statsig.com there,\n  and the public Statsig Docs MCP server at https://docs.statsig.com/api/mcp exposes a tool named\n  `amplitude_implementation_planner`. Recorded as observed evidence of a shared trust/docs\n  operation, not as a corporate-structure conclusion.\ncertifications:\n  - name: SOC 2 Type II\n    evidence: https://www.statsig.com/legal/security\n    note: \"Security at Statsig states plainly: \\\"SOC2 Type II audited and certified\\\".\"\n  - name: ISO 27001\n\
  \    evidence: https://trust.statsig.com/\n  - name: GDPR\n    evidence: https://trust.statsig.com/\n  - name: HIPAA\n    evidence: https://www.statsig.com/pricing\n    note: >-\n      The pricing page lists \"HIPAA-eligibility (BAA required)\" as an Enterprise-tier entitlement.\n      Eligibility under a BAA, not a certification.\nprograms:\n  - name: Bug Bounty Program\n    evidence: https://www.statsig.com/legal/security\n    status: named-in-prose\n    note: >-\n      Listed among SDLC testing controls. No public program page, no HackerOne or Bugcrowd listing\n      (both probed, 404), and no /.well-known/security.txt on any host — so the program exists but\n      is not reachable by a researcher who has not already been invited.\nevidence:\n  - source: https://trust.statsig.com/\n    http_status: 200\n    keywords: [trust center, soc 2, iso 27001, gdpr, compliance certification]\n  - source: https://www.statsig.com/legal/security\n    http_status: 200\n    keywords: [soc2 type ii,\
  \ bug bounty program, owasp, encryption at rest, disaster recovery]\n  - source: https://statsig.com/legal/dpa\n    http_status: 200\n    keywords: [data processing addendum]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/statsig/refs/heads/main/security/statsig-trust-center.yml
summary_line: SOC 2 Type II, ISO 27001, GDPR, HIPAA
tags:
- Feature Flags
- Experimentation
- A/B Testing
- Product Analytics
- Session Replay
- Developer Tools
- Data Warehouse
- Configuration Management
trust_url: https://trust.statsig.com/
---
