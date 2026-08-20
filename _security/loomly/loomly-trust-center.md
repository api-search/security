---
certifications: []
description: Loomly publishes a public security page rather than a hosted trust center. It describes infrastructure, encryption, testing and vendor posture, links a vulnerability reporting policy and a DPA, and names its subprocessors. It does NOT publish a customer-facing document portal, a SOC 2 report request flow, or an attestation download.
kind: trust-center
layout: security
name: Loomly Trust Center
name_suffix: Trust Center
overview: Loomly maintains a public trust center covering its security and compliance posture.
provider_name: Loomly
provider_slug: loomly
slug: loomly-trust-center
source_filename: loomly-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://www.loomly.com/security\nurl: https://www.loomly.com/security\nname: Loomly Security Page\ndescription: >-\n  Loomly publishes a public security page rather than a hosted trust center. It\n  describes infrastructure, encryption, testing and vendor posture, links a\n  vulnerability reporting policy and a DPA, and names its subprocessors. It does\n  NOT publish a customer-facing document portal, a SOC 2 report request flow, or\n  an attestation download.\ntrust_center: false\ncertifications: []\ninherited_certifications:\n  # IMPORTANT: these are the certifications of Loomly's INFRASTRUCTURE PROVIDER\n  # (AWS), quoted on Loomly's security page. They are NOT Loomly certifications\n  # and must not be credited to Loomly. A prior automated pass keyword-matched\n  # this sentence and recorded SOC 2 / ISO 27001 / PCI DSS as Loomly's own; that\n  # was wrong and is corrected here.\n  - name: ISO 27001\n    holder: AWS (Loomly's\
  \ data center provider)\n  - name: PCI DSS Service Provider Level 1\n    holder: AWS (Loomly's data center provider)\n  - name: SOC 1\n    holder: AWS (Loomly's data center provider)\n  - name: SOC 2\n    holder: AWS (Loomly's data center provider)\n  - name: SOC 3\n    holder: AWS (Loomly's data center provider)\ninherited_certifications_quote: >-\n  \"Our provider data centers are certified as ISO 27001, PCI DSS Service\n  Provider Level 1, SOC 1, SOC 2 and SOC 3 compliant.\"\nfirst_party_claims:\n  - claim: PCI-DSS compliance as a card-not-present merchant\n    detail: >-\n      Loomly states it is PCI-DSS compliant as a card-not-present merchant;\n      card data is handled by Stripe and does not touch Loomly systems.\n    scope: payments\n  - claim: Annual third-party penetration testing\n    detail: >-\n      \"Third-party penetration tests are conducted against the application and\n      supporting infrastructure at least annually.\"\n  - claim: Encryption in transit and at rest\n\
  \    detail: TLS/HTTPS enforced in transit; AES encryption at rest managed by AWS.\n  - claim: Two-factor authentication\n    detail: >-\n      2FA is available on all plans (including the free plan) and can be\n      enforced per calendar on the Beyond tier.\nsubprocessors:\n  published: true\n  source: https://www.loomly.com/security\n  named:\n    - Amazon Web Services\n    - Google\n    - HubSpot\n    - Intercom\n    - Bending Spoons\nrelated_documents:\n  - type: DataProcessingAgreement\n    url: https://www.loomly.com/dpa\n  - type: PrivacyPolicy\n    url: https://www.loomly.com/privacy\n  - type: TermsOfService\n    url: https://www.loomly.com/terms\n  - type: VulnerabilityDisclosure\n    url: https://www.loomly.com/vulnerability_reporting_policy\nevidence:\n  - url: https://www.loomly.com/security\n    http_status: 200\n    fetched: '2026-08-13'\n  - url: https://www.loomly.com/dpa\n    http_status: 200\n    fetched: '2026-08-13'\nnotes:\n  - >-\n    No SOC 2 report, ISO certificate,\
  \ or attestation of Loomly's own is offered\n    for download or on request from any public page.\n  - >-\n    No hosted trust center (Vanta/Drata/SafeBase/Conveyor) was found on any\n    loomly.com host.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/loomly/refs/heads/main/security/loomly-trust-center.yml
summary_line: trust center published
tags:
- Social-Media
- Content Calendar
- Scheduling
- Approval Workflows
- Analytics
- Brand Management
- Publishing
- Community Management
- Marketing
- Social Media Management
trust_url: https://www.loomly.com/security
---
