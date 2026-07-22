---
certifications: []
description: ''
kind: trust-center
layout: security
name: Kyrok Trust Center
name_suffix: Trust Center
overview: Kyrok maintains a public trust center covering its security and compliance posture.
provider_name: Kyrok
provider_slug: kyrok
slug: kyrok-trust-center
source_filename: kyrok-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nprobe: true\nurl: https://trust.kyrok.com/\nplatform: Vanta Trust Center (EU tenant)\nnotes: >-\n  trust.kyrok.com resolves independently (the domain has no wildcard DNS — an\n  unrelated subdomain fails to resolve) and returns a Vanta-hosted Trust Center\n  shell titled \"Kyrok Trust Center\". The report body is rendered client-side by\n  Vanta's JavaScript bundle, so the certification list could not be read from the\n  served HTML during this pass. The compliance posture recorded below is quoted\n  from Kyrok's own public homepage/FAQ, not from the Trust Center render.\ncertifications: []\ncertifications_in_progress:\n- name: ISO/IEC 27001\n  status: in progress\n  evidence: https://kyrok.com/en\n- name: ISO/IEC 42001\n  status: in progress\n  evidence: https://kyrok.com/en\ncompliance:\n- name: GDPR\n  status: claimed compliant\n  evidence: https://kyrok.com/en\ndata_residency:\n  region: EU\n  location: Frankfurt am Main, Germany\n\
  \  evidence: https://kyrok.com/en\nquotes:\n- source: https://kyrok.com/en\n  text: >-\n    In Frankfurt am Main, Germany, on European infrastructure and fully\n    GDPR-compliant. ISO certifications 27001 and 42001 are currently in progress.\nevidence:\n- source: https://trust.kyrok.com/\n  kind: vanta-trust-center\n  status: 200\n  detail: 'HTML title \"Kyrok Trust Center\"; canonical https://trust.kyrok.com'\n- source: https://kyrok.com/en\n  kind: homepage-faq\n  status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kyrok/refs/heads/main/security/kyrok-trust-center.yml
summary_line: trust center published
tags:
- Company
- Supply Chain
- Artificial Intelligence
- ERP
- Pharmaceuticals
- Chemicals
- Manufacturing
- Enterprise Software
- Germany
trust_url: https://trust.kyrok.com/
---
