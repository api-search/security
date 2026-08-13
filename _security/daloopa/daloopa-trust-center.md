---
api_specs:
- filename: daloopa-api-openapi.yml
  format: yaml
  label: Daloopa API v3
  slug: daloopa-api-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daloopa/refs/heads/main/openapi/daloopa-api-openapi.yml
- filename: daloopa-mcp-service-openapi.json
  format: json
  label: Daloopa MCP Server
  slug: daloopa-mcp-server
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daloopa/refs/heads/main/openapi/daloopa-mcp-service-openapi.json
certifications: []
description: Daloopa operates a Vanta-hosted trust center at trust.daloopa.com. Its EXISTENCE is verified; its CONTENTS are not publicly machine-readable. This artifact records exactly that boundary and names no certification that could not be read from a public source.
kind: trust-center
layout: security
name: Daloopa Trust Center
name_suffix: Trust Center
overview: Daloopa maintains a public trust center covering its security and compliance posture.
provider_name: Daloopa
provider_slug: daloopa
slug: daloopa-trust-center
source_filename: daloopa-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-11'\nmethod: probed\nsource: https://trust.daloopa.com/\ndescription: >-\n  Daloopa operates a Vanta-hosted trust center at trust.daloopa.com. Its EXISTENCE is verified; its\n  CONTENTS are not publicly machine-readable. This artifact records exactly that boundary and names no\n  certification that could not be read from a public source.\n\ntrust_center:\n  published: true\n  url: https://trust.daloopa.com/\n  vendor: Vanta\n  vendor_evidence: >-\n    Served HTML contains a `vanta-entry-loader` element and 36 references to vanta.com asset hosts. Page\n    title is \"daloopa.com Trust Center\".\n\nx-evidence:\n  fetched: '2026-08-11'\n  probes:\n  - {url: 'https://trust.daloopa.com/', http_status: 200, content_type: 'text/html', note: 'JS-rendered SPA shell; no certification text in the served markup'}\n  - {url: 'https://trust.daloopa.com/api/trustPage', http_status: 200, content_type: 'text/html', note: 'SPA catch-all, not JSON — a miss'}\n  - {url: 'https://trust.daloopa.com/api/v1/trust-center',\
  \ http_status: 200, content_type: 'text/html', note: 'SPA catch-all, not JSON — a miss'}\n  - {url: 'https://trust.daloopa.com/data.json', http_status: 200, content_type: 'text/html', note: 'SPA catch-all, not JSON — a miss'}\n  - {url: 'https://api.vanta.com/v1/trust-pages/daloopa.com', http_status: 401, content_type: 'application/json', note: 'authenticated endpoint'}\n  - {url: 'https://daloopa.com/privacy-policy', http_status: 200, note: 'GDPR referenced; no SOC 2 / ISO 27001 named'}\n  - {url: 'https://daloopa.com/terms-of-use', http_status: 200, note: 'no certification named'}\n  - {url: 'https://daloopa.com/products/api', http_status: 200, note: 'no certification named'}\n  - {url: 'https://docs.daloopa.com/docs/excel-add-in-security-and-architecture', http_status: 200, note: 'IT/infosec review page; no certification named in the markdown'}\n\ncertifications: []\ncertifications_note: >-\n  DELIBERATELY EMPTY. Every host and path above was probed and no named certification (SOC 2,\
  \ ISO 27001,\n  PCI DSS, HIPAA, FedRAMP) could be read from any public, unauthenticated source. A Vanta trust center of\n  this kind normally lists frameworks and gates the underlying reports behind an NDA request form, so it\n  is likely certifications exist — but \"likely\" is not evidence, and none are recorded here. No\n  `type: Compliance` pointer is emitted in apis.yml for the same reason.\n  If Daloopa wants this reflected, the fix on their side is small: name the frameworks in server-rendered\n  HTML, or link the trust center from a /.well-known/security.txt.\n\npublished_security_material:\n- name: Excel Add-In Security and Architecture\n  url: https://docs.daloopa.com/docs/excel-add-in-security-and-architecture\n  note: >-\n    A dedicated page describing how the add-in is built, what it can and cannot access in a desktop\n    environment, and the controls governing its behavior — written explicitly to give customer IT and\n    infosec teams what they need for approval. A genuinely\
  \ mature artifact for an Office add-in.\n- name: Privacy and Data Collection Disclosure for MCP Access\n  url: https://docs.daloopa.com/docs/daloopa-privacy-and-data-collection-disclosure-for-mcp-access\n  note: >-\n    A separate privacy disclosure written specifically for the MCP surface. Very few providers in the\n    catalog publish an agent-surface-specific privacy disclosure at all.\n- name: Single Sign-On\n  url: https://docs.daloopa.com/docs/single-sign-on\n  note: Microsoft Entra (Azure AD) SSO integration guide.\n- name: Privacy Policy\n  url: https://daloopa.com/privacy-policy\n- name: Terms of Use\n  url: https://daloopa.com/terms-of-use\n\napi_security_controls:\n  key_rotation: Published six-month API key rotation cycle.\n  ip_allowlisting: Available on request — restricts API access to pre-approved addresses.\n  source: https://docs.daloopa.com/docs/api-authentication\n\nvulnerability_disclosure:\n  published: false\n  security_txt: false\n  bug_bounty: null\n  security_contact:\
  \ null\n  note: >-\n    No security.txt on any of the five hosts, no published vulnerability disclosure or responsible\n    disclosure policy, and no HackerOne/Bugcrowd/Intigriti program found. No dedicated security@ address is\n    published; the only contact addresses are sales@, support@ and api-support@daloopa.com. No\n    VulnerabilityDisclosure artifact or `type: Security` pointer is emitted, because there is no program to\n    point at.\n\ncross_links:\n  domain_security: security/daloopa-domain-security.yml\n  well_known: well-known/daloopa-well-known.yml\n  conformance: conformance/daloopa-conformance.yml\n  authentication: authentication/daloopa-authentication.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/daloopa/refs/heads/main/security/daloopa-trust-center.yml
summary_line: trust center published
tags:
- financial-data
- fundamental-data
- market-data
- investment-research
- equity-research
- sec-filings
- earnings
- fintech
- mcp
- agent-native
- agent-skills
- webhooks
- data-warehouse
trust_url: ''
---
