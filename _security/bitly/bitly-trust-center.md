---
api_specs:
- filename: bitly-bsds-api-openapi.yml
  format: yaml
  label: Bitly BSDs API
  slug: bitly-bsds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitly/refs/heads/main/openapi/bitly-bsds-api-openapi.yml
- filename: bitly-bitlinks-api-openapi.yml
  format: yaml
  label: Bitly Bitlinks API
  slug: bitly-bitlinks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitly/refs/heads/main/openapi/bitly-bitlinks-api-openapi.yml
- filename: bitly-campaigns-api-openapi.yml
  format: yaml
  label: Bitly Campaigns API
  slug: bitly-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitly/refs/heads/main/openapi/bitly-campaigns-api-openapi.yml
- filename: bitly-custom-bitlinks-api-openapi.yml
  format: yaml
  label: Bitly Custom Bitlinks API
  slug: bitly-custom-bitlinks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitly/refs/heads/main/openapi/bitly-custom-bitlinks-api-openapi.yml
- filename: bitly-groups-api-openapi.yml
  format: yaml
  label: Bitly Groups API
  slug: bitly-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitly/refs/heads/main/openapi/bitly-groups-api-openapi.yml
- filename: bitly-oauth-apps-api-openapi.yml
  format: yaml
  label: Bitly OAuth Apps API
  slug: bitly-oauth-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitly/refs/heads/main/openapi/bitly-oauth-apps-api-openapi.yml
- filename: bitly-organizations-api-openapi.yml
  format: yaml
  label: Bitly Organizations API
  slug: bitly-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitly/refs/heads/main/openapi/bitly-organizations-api-openapi.yml
- filename: bitly-qr-codes-api-openapi.yml
  format: yaml
  label: Bitly QR Codes API
  slug: bitly-qr-codes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitly/refs/heads/main/openapi/bitly-qr-codes-api-openapi.yml
- filename: bitly-user-api-openapi.yml
  format: yaml
  label: Bitly User API
  slug: bitly-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitly/refs/heads/main/openapi/bitly-user-api-openapi.yml
- filename: bitly-webhooks-api-openapi.yml
  format: yaml
  label: Bitly Webhooks API
  slug: bitly-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitly/refs/heads/main/openapi/bitly-webhooks-api-openapi.yml
certifications:
- SOC 2 Type 2
- GDPR
- CCPA
description: ''
kind: trust-center
layout: security
name: Bitly Trust Center
name_suffix: Trust Center
overview: Bitly maintains a public trust center documenting SOC 2 Type 2, GDPR, and CCPA compliance.
provider_name: Bitly
provider_slug: bitly
slug: bitly-trust-center
source_filename: bitly-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://security.bitly.com/\nurl: https://security.bitly.com/\nname: Bitly Security & Compliance Center\nplatform: SafeBase (Drata)\naccess: gated\naccess_note: >-\n  The portal is public, but individual audit artifacts (SOC 2 report, pentest report, network\n  and data-flow diagrams, SIG self-assessment) are released on request through an approval flow\n  with delivery by secure email. The certification list itself is published without a gate.\ncertifications:\n- SOC 2 Type 2\n- GDPR\n- CCPA\ndocuments_available_on_request:\n- SOC 2 Report\n- Certificate of Engagement\n- Penetration Test Report\n- Network Diagram\n- Data Flow Diagram (DFD)\n- Information Security Policy\n- SIG Self-Assessment\n- Data Processing Agreement\n- Cyber Insurance certificate\nresilience:\n  rto: 5 minutes\n  rpo: 4 hours\nevidence:\n- source: https://security.bitly.com/\n  http_status: 200\n  kind: trust center (SafeBase-hosted, live fetch)\n  keywords:\
  \ [soc 2 type 2, gdpr, ccpa, pentest report, information security policy]\n- source: https://bitly.com/blog/bitly-soc-2-compliance/\n  kind: provider blog post announcing SOC 2 compliance\ncorrections:\n- date: '2026-08-13'\n  was: https://bitly.com/pages/landing/branded-short-domains-powered-by-bitly?bsd=trust.bitly.com\n  problem: >-\n    Prior rounds recorded trust.bitly.com as Bitly's trust center. It is not one. trust.bitly.com\n    is a registered Bitly branded short domain with no link behind it, so it 302s to the generic\n    \"Custom Domain by Bitly\" marketing landing page. That page happens to contain the string\n    \"SOC 2\" in Bitly's own marketing copy, which is what tripped the keyword probe — a soft-404\n    scored as evidence. The real trust center is the SafeBase portal at security.bitly.com,\n    which the automated probe never reaches because it is on a different subdomain.\n  resolution: >-\n    Repointed to https://security.bitly.com/ and upgraded the certification\
  \ list from\n    \"SOC 2, GDPR\" to the published SOC 2 Type 2, GDPR and CCPA.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bitly/refs/heads/main/security/bitly-trust-center.yml
summary_line: SOC 2 Type 2, GDPR, CCPA
tags:
- Links
- URL Shortener
- QR Codes
- Analytics
- Marketing
- Link Management
- Webhook
- Attribution
- Agents
- MCP
trust_url: https://security.bitly.com/
---
