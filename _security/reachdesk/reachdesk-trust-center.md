---
api_specs:
- filename: reachdesk-api-openapi.yml
  format: yaml
  label: Reachdesk API
  slug: reachdesk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reachdesk/refs/heads/main/openapi/reachdesk-api-openapi.yml
certifications:
- verified
- claimed
- note
description: Reachdesk operates a public trust center on its own subdomain, hosted by Vanta. The page exists and returns HTTP 200 with real Reachdesk-specific metadata, but its contents — the certification list, the sub-processor list and any downloadable reports — render client-side and the underlying Vanta API rejects unsigned requests. No certification is claimed in this file because none could be verified anonymously.
kind: trust-center
layout: security
name: Reachdesk Trust Center
name_suffix: Trust Center
overview: Reachdesk maintains a public trust center documenting verified, claimed, and note compliance.
provider_name: Reachdesk
provider_slug: reachdesk
slug: reachdesk-trust-center
source_filename: reachdesk-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://trust.reachdesk.com/\ndescription: >-\n  Reachdesk operates a public trust center on its own subdomain, hosted by Vanta.\n  The page exists and returns HTTP 200 with real Reachdesk-specific metadata, but\n  its contents — the certification list, the sub-processor list and any downloadable\n  reports — render client-side and the underlying Vanta API rejects unsigned\n  requests. No certification is claimed in this file because none could be verified\n  anonymously.\ntrust_center:\n  present: true\n  url: https://trust.reachdesk.com/\n  http_status: 200\n  platform: Vanta\n  canonical: https://trust.reachdesk.com\n  title: Reachdesk Trust Center\n  vanta_slug_id: xoem6skatmbuels6wgi3l\n  checked: '2026-08-13'\ncertifications:\n  verified: []\n  claimed: []\n  note: >-\n    NOT verified, not \"none\". The trust center is a Vite/React single-page app whose\n    only server-rendered content is <head> metadata. Vanta's data\
  \ endpoints answer\n    401 Unauthorized (api.vanta.com) or require a `signature`/`signedAt` pair\n    (app.vanta.com/graphql), and the legacy GraphQL API is retired (HTTP 410). A\n    human with a browser can read the certification list; an anonymous machine\n    cannot. No Compliance pointer is emitted for this provider on the strength of a\n    page whose contents were unreadable.\nprobes:\n  - url: https://trust.reachdesk.com/\n    status: 200\n    content_type: text/html\n    result: SPA shell only — no certification names present in the served HTML\n  - url: https://api.vanta.com/v1/trust-report/xoem6skatmbuels6wgi3l\n    status: 401\n    result: Unauthorized\n  - url: https://app.vanta.com/graphql\n    status: 400\n    result: 'Missing `signature` or `signedAt`'\n  - url: https://api.vanta.com/graphql\n    status: 410\n    result: GraphQL API retired in favour of the Vanta REST API\nrelated_evidence:\n  gdpr_api: >-\n    Reachdesk exposes first-class GDPR data-subject endpoints\
  \ (POST /gdpr/requests\n    for erase_subject and export_subject). That is a concrete, machine-verifiable\n    privacy capability, and it is stronger evidence than an unreadable badge wall.\n  privacy_policy: https://www.reachdesk.com/privacy-policy\n  terms: https://www.reachdesk.com/terms-and-conditions\n  cookie_policy: https://www.reachdesk.com/cookie-policy\n  scim_saml: >-\n    SCIM 2.0 provisioning and SAML SSO with Okta, Microsoft Entra ID and OneLogin\n    are documented in the knowledge base.\nvulnerability_disclosure:\n  present: false\n  note: >-\n    No security.txt on any Reachdesk host, no /security or /vulnerability-disclosure\n    page on www.reachdesk.com (both 404), and no HackerOne, Bugcrowd or Intigriti\n    program found. No Security pointer is emitted.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reachdesk/refs/heads/main/security/reachdesk-trust-center.yml
summary_line: verified, claimed, note
tags:
- Corporate Gifting
- Direct Mail
- Swag
- B2B
- Sales Enablement
- Customer Success
- Marketing Automation
- Gifting Platform
- Rewards
- MCP
- AI Agents
- OpenAPI
trust_url: ''
---
