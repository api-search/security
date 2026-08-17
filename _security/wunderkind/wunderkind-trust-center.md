---
api_specs:
- filename: wunderkind-email-api-openapi.yml
  format: yaml
  label: Wunderkind Email API
  slug: wunderkind-email-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wunderkind/refs/heads/main/openapi/wunderkind-email-api-openapi.yml
- filename: wunderkind-id-resolution-api-openapi.yml
  format: yaml
  label: Wunderkind Id Resolution API
  slug: wunderkind-id-resolution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wunderkind/refs/heads/main/openapi/wunderkind-id-resolution-api-openapi.yml
- filename: wunderkind-identity-api-openapi.yml
  format: yaml
  label: Wunderkind Identity API
  slug: wunderkind-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wunderkind/refs/heads/main/openapi/wunderkind-identity-api-openapi.yml
- filename: wunderkind-send-event-api-openapi.yml
  format: yaml
  label: Wunderkind Send Event API
  slug: wunderkind-send-event-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wunderkind/refs/heads/main/openapi/wunderkind-send-event-api-openapi.yml
- filename: wunderkind-ucrm-api-openapi.yml
  format: yaml
  label: Wunderkind Ucrm API
  slug: wunderkind-ucrm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wunderkind/refs/heads/main/openapi/wunderkind-ucrm-api-openapi.yml
- filename: wunderkind-wunderhook-api-openapi.yml
  format: yaml
  label: Wunderkind Wunderhook API
  slug: wunderkind-wunderhook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wunderkind/refs/heads/main/openapi/wunderkind-wunderhook-api-openapi.yml
certifications:
- SOC 2 Type 2
- ISO 27001
description: ''
kind: trust-center
layout: security
name: Wunderkind Trust Center
name_suffix: Trust Center
overview: Wunderkind maintains a public trust center documenting SOC 2 Type 2 and ISO 27001 compliance.
provider_name: Wunderkind
provider_slug: wunderkind
slug: wunderkind-trust-center
source_filename: wunderkind-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nprobe: true\nurl: https://trust.wunderkind.co/\nplatform: Vanta Trust Center\ncertifications:\n- SOC 2 Type 2\n- ISO 27001\ncompliance_programs:\n- GDPR\n- CCPA\n- US state privacy laws\nmemberships:\n- Network Advertising Initiative (NAI)\n- Interactive Advertising Bureau (IAB)\n- European Digital Advertising Alliance (EDAA)\ncompliance_page: https://www.wunderkind.co/blog/article/wunderkinds-commitment-to-privacy-compliance/\nnotes: >-\n  trust.wunderkind.co is live (HTTP 200) and titled \"Wunderkind Trust Center\",\n  hosted on Vanta (assets.vanta.com trust-report application, signature\n  manifest, and an app.vanta.com document link are embedded in the page shell).\n  The certification list is rendered client-side by the Vanta SPA and its\n  GraphQL backend rejects unsigned requests (\"Missing `signature` or\n  `signedAt`\", HTTP 400), so nothing is extractable from the trust center\n  itself. The certification names recorded above\
  \ are NOT taken from the trust\n  center; they come from Wunderkind's own first-party posts on wunderkind.co,\n  which state that Wunderkind \"renewed both our SOC2 and ISO 27001\n  certifications\" in 2024 and announce a SOC 2 Type 2 attestation audited by\n  A-LIGN. The privacy policy and the compliance post address GDPR, CCPA and\n  similar US state privacy laws.\nevidence:\n- source: https://trust.wunderkind.co/\n  kind: page\n  status: 200\n  detail: '<title>Wunderkind Trust Center</title>; Vanta trust-report JS application shell'\n- source: https://trust.wunderkind.co/graphql\n  kind: probe\n  status: 400\n  detail: 'Vanta trust-report GraphQL requires a signed request: {\"errors\":[{\"message\":\"Missing `signature` or `signedAt`\"}]} — certification list not machine-readable'\n- source: https://trust.wunderkind.co/\n  kind: document-link\n  detail: https://app.vanta.com/doc?s=qsm7hcih4jdrc8mrfmqsp\n- source: https://www.wunderkind.co/blog/article/wunderkinds-commitment-to-privacy-compliance/\n\
  \  kind: page\n  detail: 'first-party statement: SOC2 and ISO 27001 certifications renewed in 2024; GDPR, CCPA and similar US state privacy laws; NAI, IAB and EDAA memberships'\n- source: https://www.wunderkind.co/blog/article/soc-2-attestation/\n  kind: page\n  detail: 'first-party announcement of AICPA SOC 2 Type 2 attestation (security and confidentiality), audit performed by A-LIGN'\n- source: https://www.wunderkind.co/privacy/\n  kind: page\n  detail: GDPR referenced in the privacy policy\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wunderkind/refs/heads/main/security/wunderkind-trust-center.yml
summary_line: SOC 2 Type 2, ISO 27001
tags:
- Company
- Marketing
- Personalization
- Identity Resolution
- Email
- SMS
- Behavioral Data
- eCommerce
- Webhooks
trust_url: https://trust.wunderkind.co/
---
