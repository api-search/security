---
certifications: []
description: Flockjay operates a first-party Trust Center on its own domain covering privacy, data protection, AI data handling and security. It is real and it is public — but every answer is collapsed behind an accordion whose content is not in the served HTML, and the supporting documents are behind a lead-capture form. No certification is named anywhere on the public pages, so this profile records ZERO verified certifications and emits no Compliance pointer.
kind: trust-center
layout: security
name: Flockjay Trust Center
name_suffix: Trust Center
overview: Flockjay maintains a public trust center covering its security and compliance posture.
provider_name: Flockjay
provider_slug: flockjay
slug: flockjay-trust-center
source_filename: flockjay-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nsource: >-\n  https://flockjay.com/product/trust-center and https://flockjay.com/product/security\n  (both fetched 2026-08-14, HTTP 200)\nname: Flockjay Trust Center\ndescription: >-\n  Flockjay operates a first-party Trust Center on its own domain covering privacy,\n  data protection, AI data handling and security. It is real and it is public — but\n  every answer is collapsed behind an accordion whose content is not in the served\n  HTML, and the supporting documents are behind a lead-capture form. No certification\n  is named anywhere on the public pages, so this profile records ZERO verified\n  certifications and emits no Compliance pointer.\n\ntrust_center:\n  published: true\n  url: https://flockjay.com/product/trust-center\n  hosted: first-party\n  last_updated_on_page: '2025-06-26'\n  third_party_platform: null\n  note: >-\n    Not a Vanta/Drata/SafeBase-style hosted trust portal — a Framer page on\n    flockjay.com.\n\nsecurity_page:\n\
  \  url: https://flockjay.com/product/security\n  last_updated_on_page: '2025-02-10'\n\ntopics_covered:\n  privacy_and_data_protection:\n  - What data does the Flockjay platform collect?\n  - How does Flockjay use my data?\n  - Can Flockjay support my compliance with privacy laws?\n  - Does Flockjay share my data with other customers?\n  - Does Flockjay use AI technology?\n  - Is my data used to train AI?\n  - How long is my data stored?\n  - Who owns inputs?\n  - Does Flockjay handle personal information?\n  security:\n  - How does Flockjay ensure that my data is secure?\n  - What compliance standards does Flockjay meet?\n  note: >-\n    Question headings only. The answers are not present in the served HTML — the\n    accordion bodies are absent, so neither a human without JavaScript nor a machine\n    can read what Flockjay actually claims.\n\ncertifications: []\ncertifications_note: >-\n  NONE FOUND. The Trust Center asks \"What compliance standards does Flockjay meet?\"\n  but does\
  \ not answer it in any publicly readable form, and a full-text scan of both\n  the Trust Center and Security page HTML found no occurrence of SOC 2, ISO 27001,\n  PCI DSS, HIPAA, FedRAMP or CSA STAR. The only compliance term present anywhere in\n  the markup is \"CCPA\". Flockjay may well hold certifications; it does not publish\n  them, and this pipeline does not credit a claim it cannot read.\n\ndocuments:\n- name: Comprehensive Security Overview\n  gated: true\n  gate: lead-capture form (first name, last name, email, phone, company)\n  url: https://flockjay.com/product/security\n- name: Trust Center PDF\n  gated: partially\n  url: https://flockjay.com/share?linkId=c5ef1b82ce50ed\n  note: >-\n    Served through Flockjay's own public share-link feature — the same\n    /api/v2/sharedcontent/{id}/ endpoint the product exposes to customers. Flockjay\n    dogfoods its content-sharing surface to distribute its own trust documentation.\n\naudits:\n  third_party_audits: claimed\n  penetration_testing:\
  \ claimed\n  frequency: not stated\n  reports_available: on request (not stated publicly)\n  note: >-\n    \"Third-Party Audits\" and \"Third-Party Penetration Testing\" appear as control\n    headings on the security page. No auditor, scope, date or report availability is\n    published.\n\ndata_residency: not published\nsubprocessors: not published\nsubprocessor_page: null\n\nevidence:\n- url: https://flockjay.com/product/trust-center\n  status: 200\n- url: https://flockjay.com/product/security\n  status: 200\n- url: https://flockjay.com/legal/privacy-policy\n  status: 200\n- url: https://flockjay.com/legal/terms-and-conditions\n  status: 200\n\nfindings:\n- >-\n  The gap between having a Trust Center and being verifiably compliant is the whole\n  story here. Flockjay built the page, listed the right control families, and then\n  put every answer behind an accordion that does not render server-side and every\n  document behind a form.\n- >-\n  Naming its certifications in plain text\
  \ on the Trust Center page would be the single\n  cheapest credibility improvement available to this company.\n\nrelated:\n  vulnerability_disclosure: security/flockjay-vulnerability-disclosure.yml\n  domain_security: security/flockjay-domain-security.yml\n  conformance: conformance/flockjay-conformance.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flockjay/refs/heads/main/security/flockjay-trust-center.yml
summary_line: trust center published
tags:
- Company
- Sales Enablement
- Sales Training
- Learning Management
- Revenue Operations
- AI Coaching
- Content Management
- SaaS
- MCP
- Agent Native
- OAuth
trust_url: ''
---
