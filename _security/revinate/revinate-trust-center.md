---
api_specs:
- filename: revinate-porter-openapi.yml
  format: yaml
  label: Revinate Porter API
  slug: porter
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revinate/refs/heads/main/openapi/revinate-porter-openapi.yml
certifications: []
description: ''
kind: trust-center
layout: security
name: Revinate Trust Center
name_suffix: Trust Center
overview: Revinate maintains a public trust center covering its security and compliance posture.
provider_name: Revinate
provider_slug: revinate
slug: revinate-trust-center
source_filename: revinate-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: https://trust.revinate.com/\npresent: true\nvendor: Vanta\nnote: >-\n  Revinate operates a hosted Trust Center at trust.revinate.com, linked directly from the\n  www.revinate.com homepage footer and returning HTTP 200. It is Revinate's authoritative compliance\n  surface — the marketing site's /privacy-policy/ URL redirects into it as a resource\n  (trust.revinate.com/resources?...&name=revinate-solutions-privacy-policy), which confirms the\n  tenant is genuinely Revinate's and actively used.\n  HONEST LIMIT: the certification list could NOT be enumerated. The Trust Center is a fully\n  client-side-rendered Vanta single-page application whose catch-all answers HTTP 200 with the same\n  HTML shell for every path, including /api/trust-center and /resources. No certification name is\n  present anywhere in the served HTML. Certifications are therefore recorded as unverified rather\n  than guessed — no SOC 2, ISO 27001 or PCI claim\
  \ has been asserted on Revinate's behalf.\ncertifications: []\ncertifications_verified: false\ncertifications_unreadable_reason: js-rendered\nevidence:\n- url: https://trust.revinate.com/\n  status: 200\n  note: Title \"Revinate Trust Center\". Vanta-hosted (assets.vanta.com signature manifest in the document head).\n- url: https://www.revinate.com/privacy-policy/\n  status: 200\n  note: 302s into trust.revinate.com/resources with a real Revinate resource identifier.\n- url: https://trust.revinate.com/api/trust-center\n  status: 200\n  note: Returns the SPA HTML shell, not JSON. No machine-readable certification data available anonymously.\ndocuments:\n- name: Revinate Solutions Privacy Policy\n  hosted_on: trust.revinate.com\n  url: https://www.revinate.com/privacy-policy/\nrecommendation: >-\n  For the provider — a Vanta Trust Center can be configured to expose a public, crawlable summary of\n  active certifications. Enabling it, or listing certification names in server-rendered HTML,\
  \ would\n  make Revinate's compliance posture machine-readable to procurement tooling and AI agents that\n  cannot execute JavaScript.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/revinate/refs/heads/main/security/revinate-trust-center.yml
summary_line: trust center published
tags:
- Hospitality
- Hotels
- Reviews
- Reputation Management
- Guest Data Platform
- CRM
- Sentiment Analysis
- Travel
- Marketing
- Customer Feedback
trust_url: ''
---
