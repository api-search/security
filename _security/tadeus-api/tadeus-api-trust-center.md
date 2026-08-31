---
api_specs:
- filename: tadeus-api-attempts-api-openapi.yml
  format: yaml
  label: Tadeus API Attempts API
  slug: tadeus-api-attempts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tadeus-api/refs/heads/main/openapi/tadeus-api-attempts-api-openapi.yml
- filename: tadeus-api-billing-api-openapi.yml
  format: yaml
  label: Tadeus API Billing API
  slug: tadeus-api-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tadeus-api/refs/heads/main/openapi/tadeus-api-billing-api-openapi.yml
- filename: tadeus-api-campaigns-api-openapi.yml
  format: yaml
  label: Tadeus API Campaigns API
  slug: tadeus-api-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tadeus-api/refs/heads/main/openapi/tadeus-api-campaigns-api-openapi.yml
- filename: tadeus-api-insights-api-openapi.yml
  format: yaml
  label: Tadeus API Insights API
  slug: tadeus-api-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tadeus-api/refs/heads/main/openapi/tadeus-api-insights-api-openapi.yml
- filename: tadeus-api-organisation-api-openapi.yml
  format: yaml
  label: Tadeus API Organisation API
  slug: tadeus-api-organisation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tadeus-api/refs/heads/main/openapi/tadeus-api-organisation-api-openapi.yml
- filename: tadeus-api-results-api-openapi.yml
  format: yaml
  label: Tadeus API Results API
  slug: tadeus-api-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tadeus-api/refs/heads/main/openapi/tadeus-api-results-api-openapi.yml
- filename: tadeus-api-sessions-api-openapi.yml
  format: yaml
  label: Tadeus API Sessions API
  slug: tadeus-api-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tadeus-api/refs/heads/main/openapi/tadeus-api-sessions-api-openapi.yml
- filename: tadeus-api-templates-api-openapi.yml
  format: yaml
  label: Tadeus API Templates API
  slug: tadeus-api-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tadeus-api/refs/heads/main/openapi/tadeus-api-templates-api-openapi.yml
- filename: tadeus-api-transcripts-api-openapi.yml
  format: yaml
  label: Tadeus API Transcripts API
  slug: tadeus-api-transcripts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tadeus-api/refs/heads/main/openapi/tadeus-api-transcripts-api-openapi.yml
certifications:
- count
- audited
- claimed
- note
description: Tadeus runs a public, ungated trust surface built entirely around the EU AI Act rather than around security certifications. It publishes versioned, dated documents with a review date on each, describes itself as "data-room style", and serves every document as plain markdown at its URL plus ".md" so machines can read it. It also ships a free, no-sign-up interactive classifier that walks a buyer through Article 5, Article 6(1), all eight Annex III categories and the Article 50 duties, and pre-fills a memo.
kind: trust-center
layout: security
name: Tadeus Api Trust Center
name_suffix: Trust Center
overview: Tadeus API maintains a public trust center documenting count, audited, claimed, and note compliance.
provider_name: Tadeus API
provider_slug: tadeus-api
slug: tadeus-api-trust-center
source_filename: tadeus-api-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-11'\nmethod: searched\nsource: https://tadeus.net/trust\npresent: true\nname: Tadeus Trust — Compliance tools and documents\nurl: https://tadeus.net/trust\ntype: self-published-document-library\ngated: false\nsign_in_required: false\ndescription: >-\n  Tadeus runs a public, ungated trust surface built entirely around the EU AI Act rather\n  than around security certifications. It publishes versioned, dated documents with a\n  review date on each, describes itself as \"data-room style\", and serves every document as\n  plain markdown at its URL plus \".md\" so machines can read it. It also ships a free,\n  no-sign-up interactive classifier that walks a buyer through Article 5, Article 6(1),\n  all eight Annex III categories and the Article 50 duties, and pre-fills a memo.\ndocuments:\n  - title: How Tadeus Classifies Itself Under the EU AI Act\n    kind: self-classification\n    version: '1.2'\n    reviewed: '2026-07-15'\n    formats: [html, md]\n    url:\
  \ https://tadeus.net/trust/how-tadeus-classifies-itself\n    markdown_url: https://tadeus.net/trust/how-tadeus-classifies-itself.md\n    markdown_status: 200\n  - title: Tadeus Instructions for Use (Article 13)\n    kind: instructions-for-use\n    version: '1.1'\n    reviewed: '2026-07-15'\n    formats: [html, md]\n    url: https://tadeus.net/trust/instructions-for-use\n    markdown_url: https://tadeus.net/trust/instructions-for-use.md\n    markdown_status: 200\n    note: Published ahead of the December 2027 obligation.\n  - title: The EU AI Act Classification Framework for Workforce AI\n    kind: framework\n    version: '1.1'\n    reviewed: '2026-07-11'\n    url: https://tadeus.net/trust/classification-framework\n  - title: EU AI Act Classification Memo Template\n    kind: template\n    version: '1.1'\n    reviewed: '2026-07-11'\n    formats: [md, docx]\n    url: https://tadeus.net/trust/classification-framework#memo-template\ntools:\n  - name: EU AI Act Classifier for Workforce AI\n\
  \    version: '3.0'\n    reviewed: '2026-07-15'\n    url: https://tadeus.net/trust/ai-act-classifier\n    free: true\n    sign_up_required: false\ncertifications:\n  count: 0\n  audited: []\n  claimed: []\n  note: >-\n    No third-party attestation of any kind is claimed — no SOC 2, ISO 27001, ISO 42001,\n    HIPAA, PCI DSS or FedRAMP. This is the defining characteristic of the Tadeus trust\n    surface: deep regulatory documentation, zero independent audit.\nsecurity_practices_claimed:\n  source: https://tadeus.net/\n  claims:\n    - No audio retained — the system works from the transcript; raw audio is never stored.\n    - No video or facial biometrics.\n    - Comprehension and engagement signals, not emotion inference.\n    - Region-gated configuration so EU deployments stay clear of the AI Act line.\n    - Data encrypted in transit and at rest.\n    - Models are not trained on customer data.\n    - Privacy-friendly EU-hosted analytics (PostHog), consent-gated.\n  enterprise_tier_only:\n\
  \    - SSO and SAML\n    - EU data residency\n    - DPA\n    - SLA\n    - security review\nobserved_transport_posture:\n  source: live probe 2026-08-11\n  https_only: true\n  tls: TLSv1.3\n  hsts: false\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n  note: >-\n    See security/tadeus-api-domain-security.yml. Worth reading against the trust claims:\n    there is no HSTS, no DNSSEC, no CAA record, and DMARC is at p=none (monitor only, no\n    enforcement) on the domain of a vendor selling into regulated workplaces.\nvulnerability_disclosure:\n  present: false\n  see: security/tadeus-api-vulnerability-disclosure.yml\nprovider_gaps:\n  - Obtain and publish a third-party attestation (ISO 27001 and/or ISO 42001).\n  - Publish a vulnerability disclosure policy and a security.txt.\n  - Move DMARC from p=none to p=quarantine or p=reject; add HSTS, CAA and DNSSEC.\n  - Publish the DPA and SLA rather than gating them behind an Enterprise conversation.\nx-evidence:\n\
  \  fetched: '2026-08-11'\n  evidence:\n    - url: https://tadeus.net/trust\n      http_status: 200\n    - url: https://tadeus.net/trust/instructions-for-use\n      http_status: 200\n    - url: https://tadeus.net/trust/instructions-for-use.md\n      http_status: 200\n    - url: https://tadeus.net/trust/how-tadeus-classifies-itself.md\n      http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tadeus-api/refs/heads/main/security/tadeus-api-trust-center.yml
summary_line: count, audited, claimed, note
tags:
- Voice AI
- Research
- Interviews
- Workforce
- HR Tech
- Conversational AI
- Employee Experience
- AI Agents
- MCP
- EU AI Act
- Compliance
- Employee Engagement
trust_url: https://tadeus.net/trust
---
