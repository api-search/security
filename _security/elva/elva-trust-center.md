---
certification_count: 3
certifications:
- SOC 2 Type II
- ISO 27001
- ISO 27701
description: ''
kind: trust-center
layout: security
name: Elva Trust Center
name_suffix: Trust Center
overview: Elva maintains a public trust center documenting SOC 2 Type II, ISO 27001, and ISO 27701 compliance.
provider_name: Elva
provider_slug: elva
slug: elva-trust-center
source_filename: elva-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: searched\nsource: https://getelva.ai/security\nname: Elva security page (Theneo-held certifications)\nnote: >-\n  Elva publishes a dedicated security page rather than a hosted trust-center portal.\n  It states plainly that Elva is a product of Theneo and that the certifications,\n  security contact, and DPA are issued to Theneo, covering the infrastructure Elva\n  runs on. Security pack (reports, certificates, pen-test summary) available on\n  request via hello@getelva.ai, under NDA.\ncertifications:\n  - name: SOC 2 Type II\n    status: certified\n    holder: Theneo\n    detail: report under NDA\n  - name: ISO 27001\n    status: certified\n    holder: Theneo\n    detail: certificates on request\n  - name: ISO 27701\n    status: certified\n    holder: Theneo\n    detail: privacy management, certificates on request\nprograms:\n  - name: GDPR\n    status: compliant\n    detail: DPA available, EU data residency on request\n  - name: Penetration\
  \ testing\n    status: annual\n    detail: third-party, summary shared under NDA\ncontrols:\n  - Encryption TLS 1.3 in transit, AES-256 at rest, per-tenant isolation\n  - SSO / SAML and SCIM on Enterprise plans\n  - Configurable data residency (regional hosting, private cloud, on-prem)\n  - Five ordered checks on every MCP tool call (identity, scope, redaction, rate, audit), fail closed\n  - Request/response bodies not retained by default; PII redacted at the gateway\n  - Instant revocation of keys, agents, and servers; full audit log export (JSON, CSV, webhook)\nevidence:\n  - url: https://getelva.ai/security\n    http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/elva/refs/heads/main/security/elva-trust-center.yml
summary_line: SOC 2 Type II, ISO 27001, ISO 27701
tags:
- API Management
- MCP Server
- MCP Logs
- MCP Insights
- API Client
- API Contract
- API Governance
- API Discovery
- OpenAPI
- API Testing
- Developer Tools
- AI Agent Infrastructure
trust_url: ''
---
