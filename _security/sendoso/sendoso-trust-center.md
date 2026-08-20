---
api_specs:
- filename: sendoso-core-api-openapi.yml
  format: yaml
  label: Sendoso Core API
  slug: sendoso-core-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendoso/refs/heads/main/openapi/sendoso-core-api-openapi.yml
- filename: sendoso-marketplace-api-openapi.yml
  format: yaml
  label: Sendoso Marketplace and SmartSend API
  slug: sendoso-marketplace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendoso/refs/heads/main/openapi/sendoso-marketplace-api-openapi.yml
- filename: sendoso-scim-api-openapi.yml
  format: yaml
  label: Sendoso SCIM API
  slug: sendoso-scim-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendoso/refs/heads/main/openapi/sendoso-scim-api-openapi.yml
- filename: sendoso-webhooks-asyncapi.yml
  format: yaml
  label: Sendoso Webhooks
  slug: sendoso-webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendoso/refs/heads/main/asyncapi/sendoso-webhooks-asyncapi.yml
certifications: []
description: 'Sendoso runs a Vanta-hosted Trust Center at security.sendoso.com. It answers HTTP 200, but it is a client-rendered single-page application: the 5.7 KB HTML the server actually delivers contains the title "Sendoso Trust Center" and nothing else — no certification name, no control, no document list. Certifications are therefore NOT recorded here, because none were readable. That is a measurement of the surface, not a claim about Sendoso''s compliance posture.'
kind: trust-center
layout: security
name: Sendoso Trust Center
name_suffix: Trust Center
overview: Sendoso maintains a public trust center covering its security and compliance posture.
provider_name: Sendoso
provider_slug: sendoso
slug: sendoso-trust-center
source_filename: sendoso-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://security.sendoso.com/\nprovider: Sendoso\nproviderId: sendoso\ndescription: >-\n  Sendoso runs a Vanta-hosted Trust Center at security.sendoso.com. It answers HTTP 200, but\n  it is a client-rendered single-page application: the 5.7 KB HTML the server actually\n  delivers contains the title \"Sendoso Trust Center\" and nothing else — no certification\n  name, no control, no document list. Certifications are therefore NOT recorded here, because\n  none were readable. That is a measurement of the surface, not a claim about Sendoso's\n  compliance posture.\ntrust_center:\n  url: https://security.sendoso.com/\n  http_status: 200\n  platform: Vanta\n  platform_evidence: >-\n    Page assets load exclusively from assets.vanta.com (index-trust-report bundle), and the\n    page links a Vanta document viewer at https://app.vanta.com/doc?s=wj3tcv6rtc7222p39ikj9.\n  discovered_via: https://www.sendoso.com/security (302 to security.sendoso.com)\n\
  \  machine_readable: false\n  machine_readable_note: >-\n    Probed for a machine-readable trust report at /api/trust-center, /api/trust-report,\n    app.vanta.com/api/trust-report/sendoso and app.vanta.com/api/trust/sendoso — all returned\n    the SPA HTML shell rather than data.\ncertifications: []\ncertifications_note: >-\n  None readable. Do not emit a Compliance pointer from this file; a trust center whose\n  contents cannot be read is not published evidence of a named certification.\ncompliance_signals_found_elsewhere:\n  - signal: CCPA\n    where: https://www.sendoso.com/ and https://www.sendoso.com/compare-plans (footer link)\n    note: A privacy-rights link, not a certification.\n  - signal: Anti-Bribery Controls\n    where: https://www.sendoso.com/compare-plans\n    note: Sold as an Enterprise-tier feature row, not stated as an external attestation.\n  - signal: Advanced Audit Services\n    where: https://www.sendoso.com/compare-plans\n    note: Enterprise-tier feature row.\n\
  security_claims_in_docs:\n  - claim: Data encrypted at rest with AES-256.\n    source: https://developer.sendoso.com/rest-api/overview/security\n  - claim: Data in transit over HTTPS TLS 1.2 with RSA 256-bit.\n    source: https://developer.sendoso.com/rest-api/overview/security\n    observed: TLSv1.3 negotiated on all three hosts (probed 2026-08-13).\n  - claim: >-\n      All API requests are logged (IP, method, resource, response status) and monitored for\n      suspicious activity.\n    source: https://developer.sendoso.com/rest-api/overview/security\nenterprise_controls_published:\n  source: https://www.sendoso.com/compare-plans\n  controls:\n    - Single Sign-On (SSO) — Core tier and above\n    - SCIM user management — Enterprise tier\n    - IP allow listing — Enterprise tier\n    - Admin audit log — Enterprise tier\n    - Policy Center — Enterprise tier\n    - Advanced IT controls — Enterprise tier\nrecommendation_for_provider: >-\n  The Vanta trust center is invisible to every automated\
  \ reader, including the AI agents\n  Sendoso is otherwise courting with an MCP server and an agent skill. Serving the\n  certification list as static HTML, or exposing Vanta's public trust-report JSON, would make\n  a real compliance program legible without changing what is disclosed.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sendoso/refs/heads/main/security/sendoso-trust-center.yml
summary_line: trust center published
tags:
- Corporate Gifting
- Direct Mail
- Sales Engagement
- Marketing Automation
- CRM Integration
- eGifts
- Swag and Merchandise
- Fulfillment
- Employee Recognition
- Account Based Marketing
- SCIM Provisioning
- Webhook
trust_url: ''
---
