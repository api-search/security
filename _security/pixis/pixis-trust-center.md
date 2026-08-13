---
certifications:
- SOC 2
- ISO
description: 'Pixis publishes a product page that names three compliance regimes. It is a marketing page, not a trust center: there is no portal, no report request flow, no subprocessor list, no certificate number, no audit period, and no named auditor. Recorded here because the claims are real and provider-published, and because the gap between the claim and the evidence is itself the finding.'
kind: trust-center
layout: security
name: Pixis Trust Center
name_suffix: Trust Center
overview: Pixis maintains a public trust center documenting SOC 2 and ISO compliance.
provider_name: Pixis
provider_slug: pixis
slug: pixis-trust-center
source_filename: pixis-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: https://pixis.ai/products/compliance/\nname: Pixis — compliance posture\ndescription: >-\n  Pixis publishes a product page that names three compliance regimes. It is a marketing page,\n  not a trust center: there is no portal, no report request flow, no subprocessor list, no\n  certificate number, no audit period, and no named auditor. Recorded here because the claims\n  are real and provider-published, and because the gap between the claim and the evidence is\n  itself the finding.\n\ntrust_center:\n  present: false\n  url: null\n  note: >-\n    No trust.pixis.ai, security.pixis.ai, Vanta/Drata/SafeBase/Conveyor portal, or \"request our\n    SOC 2 report\" flow found. https://pixis.ai/products/compliance/ (HTTP 200) is the only\n    compliance surface.\n\ncertifications:\n  - name: SOC 2\n    status: claimed\n    detail: >-\n      \"We adhere to rigorous security, availability, and confidentiality controls when it comes\n\
  \      to handling sensitive data.\"\n    type_stated: false\n    report_available: false\n    auditor: null\n    period: null\n    source: https://pixis.ai/products/compliance/\n  - name: ISO\n    status: claimed\n    detail: >-\n      \"Our processes meet internationally recognized security and data management standards,\n      ensuring the highest level of protection.\"\n    standard_number_stated: false\n    certificate_available: false\n    certifying_body: null\n    source: https://pixis.ai/products/compliance/\n    note: >-\n      The page says only \"ISO\". It does not say ISO/IEC 27001, 27017, 27018 or 42001, so the\n      specific standard cannot be recorded without guessing.\n\nregulatory:\n  - name: GDPR\n    status: claimed\n    detail: '\"Pixis is fully compliant with GDPR regulations, ensuring personal data is handled with transparency, integrity, and user consent.\"'\n    source: https://pixis.ai/products/compliance/\n  - name: Privacy policy\n    status: published\n  \
  \  url: https://pixis.ai/privacy-policy/\n    http_status: 200\n\nnot_found:\n  - CCPA/CPRA statement\n  - HIPAA\n  - PCI DSS\n  - FedRAMP\n  - Data processing agreement (DPA) at a public URL\n  - Subprocessor list\n  - Terms of service page (no /terms path in the pixis.ai sitemap, 547 URLs enumerated)\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pixis/refs/heads/main/security/pixis-trust-center.yml
summary_line: SOC 2, ISO
tags:
- Company
- Enterprise
- Advertising
- Marketing
- Artificial Intelligence
- Generative AI
- Advertising Technology
- Marketing Automation
trust_url: ''
---
