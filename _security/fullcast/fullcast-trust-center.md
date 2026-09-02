---
api_specs:
- filename: fullcast-copilot-api-api-openapi.yml
  format: yaml
  label: Fullcast Copilot API
  slug: fullcast-copilot-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fullcast/refs/heads/main/openapi/fullcast-copilot-api-api-openapi.yml
- filename: fullcast-mcp-info-api-openapi.yml
  format: yaml
  label: Fullcast Mcp Info API
  slug: fullcast-mcp-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fullcast/refs/heads/main/openapi/fullcast-mcp-info-api-openapi.yml
- filename: fullcast-oauth-api-openapi.yml
  format: yaml
  label: Fullcast OAUTH API
  slug: fullcast-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fullcast/refs/heads/main/openapi/fullcast-oauth-api-openapi.yml
- filename: fullcast-well-known-api-openapi.yml
  format: yaml
  label: Fullcast .well Known API
  slug: fullcast-well-known-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fullcast/refs/heads/main/openapi/fullcast-well-known-api-openapi.yml
certifications:
- SOC 2 Type 2
- GDPR
description: ''
kind: trust-center
layout: security
name: Fullcast Trust Center
name_suffix: Trust Center
overview: Fullcast maintains a public trust center documenting SOC 2 Type 2 and GDPR compliance.
provider_name: Fullcast
provider_slug: fullcast
slug: fullcast-trust-center
source_filename: fullcast-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nprobe: true\nurl: https://trust.fullcast.io/\naliases:\n- https://trust.fullcast.com\nplatform: Vanta\nnote: >-\n  trust.fullcast.com 301-redirects to trust.fullcast.io, a Vanta-hosted trust center. The\n  page is fully client-rendered -- the served HTML carries only the title\n  \"Fullcast.com Trust Center\" (25 characters of text), so the certification list, control\n  categories and subprocessors are not machine-readable and could not be captured. The\n  certifications below are therefore taken from the provider's own security page, which is\n  server-rendered, and NOT from the trust center itself. The prior pass recorded a\n  \"responsible disclosure\" program; a re-read of the security page on 2026-08-13 found a\n  dedicated security team and incident response but no published disclosure process, security\n  contact address or bug-bounty program, and no security.txt on any host -- so that claim is\n  downgraded here and no Security\
  \ pointer is emitted in apis.yml.\ncertifications:\n- SOC 2 Type 2\n- GDPR\nprograms:\n- incident response (SOC 2 Type 2 aligned)\nsecurity_controls_published:\n- data sovereignty / customer-controlled hosting location\n- encryption at every stage\n- multi-factor authentication\n- role-based access control with granular permissions\n- audit trails with SIEM integration\ndisclosure:\n  policy_url: null\n  security_contact: null\n  bug_bounty: false\n  security_txt: false\n  evidence: >-\n    /.well-known/security.txt returned 404 on www.fullcast.com, app.fullcast.io,\n    support.fullcast.com, assistant.fullcast.io and api.copy.ai on 2026-08-13.\nevidence:\n- source: https://www.fullcast.com/security/\n  status: 200\n  keywords: [soc 2 type 2, gdpr, encryption, mfa, rbac, audit trail, incident response]\n- source: https://trust.fullcast.io/\n  status: 200\n  keywords: [trust center]\n  machine_readable: false\n  reason: js-rendered (Vanta); 25 characters of server-rendered text\n- source:\
  \ https://trust.fullcast.com\n  status: 301\n  redirects_to: https://trust.fullcast.io/\ngaps:\n- No ISO 27001, HIPAA, PCI DSS or FedRAMP certification is claimed.\n- No security.txt, no published vulnerability disclosure policy, no security contact address.\n- Trust center content is not machine-readable, so certifications cannot be verified at the source.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fullcast/refs/heads/main/security/fullcast-trust-center.yml
summary_line: SOC 2 Type 2, GDPR
tags:
- Company
- Enterprise
- Revenue Operations
- Sales Planning
- Territory Management
- Go-To-Market
- Incentive Compensation
- Forecasting
- Lead Routing
- MCP
- AI Agents
- Sales Compensation
trust_url: https://trust.fullcast.io/
---
