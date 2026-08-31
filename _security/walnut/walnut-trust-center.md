---
certifications:
- SOC 2 Type II
- GDPR
- CCPA
description: 'Walnut runs a dedicated trust center at security.walnut.io, linked from its public Legal Hub. The portal is a HyperComply-hosted single-page application: it answers HTTP 200 but renders its content client-side through an Apollo GraphQL client, so the certification list, sub-processor register and document requests cannot be read without executing JavaScript. The certifications recorded below are therefore taken from Walnut''s own machine-readable and human-readable pages, not scraped from the portal shell.'
kind: trust-center
layout: security
name: Walnut Trust Center
name_suffix: Trust Center
overview: Walnut maintains a public trust center documenting SOC 2 Type II, GDPR, and CCPA compliance.
provider_name: Walnut
provider_slug: walnut
slug: walnut-trust-center
source_filename: walnut-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "name: Walnut Trust Center\ndescription: >-\n  Walnut runs a dedicated trust center at security.walnut.io, linked from its public Legal Hub.\n  The portal is a HyperComply-hosted single-page application: it answers HTTP 200 but renders its\n  content client-side through an Apollo GraphQL client, so the certification list, sub-processor\n  register and document requests cannot be read without executing JavaScript. The certifications\n  recorded below are therefore taken from Walnut's own machine-readable and human-readable pages,\n  not scraped from the portal shell.\ngenerated: '2026-08-13'\nmethod: searched\nsource: https://security.walnut.io/\nchecked: '2026-08-13'\n\ntrust_center:\n  url: https://security.walnut.io/\n  http_status: 200\n  platform: HyperComply\n  machine_readable: false\n  render: client-side (JavaScript required; \"You need to enable JavaScript to run this app.\")\n  discovered_via: https://www.walnut.io/legal-hub/\n  gated: >-\n    Document access on a\
  \ HyperComply portal typically requires a request or NDA. Not tested — no\n    request was submitted.\n\ncertifications:\n  - name: SOC 2 Type II\n    status: certified\n    scope: not published publicly\n    evidence:\n      - url: https://www.walnut.io/llms.txt\n        quote: '\"**Compliance**: SOC 2 Type II, GDPR.\"'\n        status: 200\n      - url: https://www.walnut.io/product/enterprise/\n        quote: '\"We''re SOC 2 certified, which means you can share your demos with the peace of mind that your customers'' data is safe.\"'\n        status: 200\n    report_available: >-\n      Not published openly. A SOC 2 report would be requested through security.walnut.io or the\n      Walnut account team.\n  - name: GDPR\n    status: compliance program\n    type: regulation\n    evidence:\n      - url: https://www.walnut.io/llms.txt\n        status: 200\n      - url: https://www.walnut.io/dpa/\n        status: 200\n        note: Data Processing Agreement published on the Legal Hub.\n  -\
  \ name: CCPA\n    status: compliance program\n    type: regulation\n    evidence:\n      - url: https://www.walnut.io/ccpa/\n        status: 200\n        note: CCPA Notice published on the Legal Hub.\n\nnot_claimed:\n  - ISO 27001\n  - PCI DSS\n  - HIPAA\n  - FedRAMP\n  - TISAX\n  - CSA STAR\nnot_claimed_note: >-\n  No claim to any of these was found on walnut.io, help.walnut.io or in Walnut's llms.txt. Their\n  absence here means \"not found\", not \"does not hold\" — the trust center itself is JS-rendered\n  and may list more.\n\nlegal_documents:\n  - name: Master Services Agreement\n    url: https://www.walnut.io/msa/\n    status: 200\n  - name: Data Processing Agreement\n    url: https://www.walnut.io/dpa/\n    status: 200\n  - name: Privacy Policy\n    url: https://www.walnut.io/privacy/\n    status: 200\n  - name: Acceptable Use Policy\n    url: https://www.walnut.io/acceptable-use-policy/\n    status: 200\n  - name: AI Terms & Conditions\n    url: https://www.walnut.io/ai-terms-conditions/\n\
  \    status: 200\n  - name: CCPA Notice\n    url: https://www.walnut.io/ccpa/\n    status: 200\n  - name: Cookies List\n    url: https://www.walnut.io/cookies-list/\n    status: 200\n  - name: Legal Hub (index)\n    url: https://www.walnut.io/legal-hub/\n    status: 200\n\nenterprise_security_features:\n  - SSO (SAML) — Accelerate and Scale plans\n  - SCIM provisioning — Accelerate and Scale plans\n  - Role-based access control (Account Owner, Admin, Editor, Presenter, Collaborator)\n  - Access gates and access codes on demos, Playlists and Deal Rooms\n  - Allow and block lists for demo viewers\n  - White-labeled / custom-domain demo delivery\n\nenterprise_security_features_source: https://www.walnut.io/product/enterprise/\n\ngaps:\n  - >-\n    No security.txt at /.well-known/security.txt on any Walnut host, so there is no machine-\n    discoverable route from an API host to this trust center. See well-known/walnut-well-known.yml.\n  - >-\n    No public sub-processor list, penetration-test\
  \ summary, or uptime/SLA commitment reachable\n    without JavaScript.\n  - No published vulnerability disclosure policy or bug bounty program (see notes below).\n\nvulnerability_disclosure:\n  found: false\n  note: >-\n    Probed 2026-08-13. No /.well-known/security.txt on www.walnut.io, help.walnut.io,\n    app.teamwalnut.com, customer-api.teamwalnut.com or api.teamwalnut.com; no HackerOne,\n    Bugcrowd or Intigriti program found; no /security or /responsible-disclosure page on\n    walnut.io (https://www.walnut.io/security returned 404). A disclosure policy may exist behind\n    the JS-rendered trust center, but nothing is publicly readable, so no\n    security/walnut-vulnerability-disclosure.yml artifact and no `Security` pointer is emitted.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/walnut/refs/heads/main/security/walnut-trust-center.yml
summary_line: SOC 2 Type II, GDPR, CCPA
tags:
- Sales Demo
- Interactive Demos
- Product Demos
- Sales Enablement
- Demo Analytics
- Go-to-Market
- AI-Powered
- Webhook
- MCP
- Analytics
trust_url: ''
---
