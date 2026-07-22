---
certifications: []
description: ''
kind: trust-center
layout: security
name: Lightbeam Ai Trust Center
name_suffix: Trust Center
overview: Lightbeam maintains a public trust center covering its security and compliance posture.
provider_name: Lightbeam
provider_slug: lightbeam-ai
slug: lightbeam-ai-trust-center
source_filename: lightbeam-ai-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nprobe: true\nsource: https://www.lightbeam.ai/trust/\nurl: https://www.lightbeam.ai/trust/\n# CORRECTION (2026-07-19 manual review): the automated probe read PCI DSS / HIPAA /\n# GDPR off this page and recorded them as certifications held. Manual review of the\n# rendered page shows those strings come from the site-wide \"Solutions > Regulations\"\n# navigation menu, not from any attestation Lightbeam publishes about itself. The\n# page titled \"Trust Center\" is in substance a privacy policy (data collected, how it\n# is used, storage/retention, data-subject rights). No named certification (SOC 2,\n# ISO 27001, PCI DSS, HIPAA, FedRAMP, HITRUST) is claimed for Lightbeam itself, and\n# no subprocessor list or third-party trust portal is linked from it.\ncertifications: []\ncertifications_published: false\nsubprocessor_list: false\ntrust_portal: false\nnotes: >-\n  Page is a privacy policy published under the \"Trust Center\" title.\
  \ Regulatory\n  frameworks named on the page (GDPR, CCPA, PCI/DSS, Quebec Law 25, HIPAA) are\n  the compliance outcomes the Lightbeam product helps customers address - they\n  are solution pages, not attestations the company holds.\nregulatory_solution_areas:\n- name: GDPR\n  url: https://www.lightbeam.ai/solutions/regulations/gdpr/\n- name: CCPA\n  url: https://www.lightbeam.ai/solutions/regulations/ccpa/\n- name: HIPAA\n  url: https://www.lightbeam.ai/solutions/regulations/hipaa/\n- name: Quebec Law 25\n  url: https://www.lightbeam.ai/solutions/regulations/quebecs-law-25/\n- name: EU AI Act\n  url: https://www.lightbeam.ai/privacy/eu-ai-act-compliance/\n- name: PCI DSS\n  url: https://www.lightbeam.ai/solutions/regulations/\nprivacy_contact_documented: true\nevidence:\n- source: https://www.lightbeam.ai/trust/\n  http_status: 200\n  finding: >-\n    Privacy policy content; data-subject rights process with a stated one-month\n    response target and a privacy email contact. No certification\
  \ names asserted\n    for Lightbeam as an organization.\n- source: https://www.lightbeam.ai/page-sitemap.xml\n  http_status: 200\n  finding: Regulation solution pages enumerated (GDPR, CCPA, HIPAA, Law 25, EU AI Act).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lightbeam-ai/refs/heads/main/security/lightbeam-ai-trust-center.yml
summary_line: trust center published
tags:
- Company
- Security
- Data Security
- Data Security Posture Management
- Data Classification
- Privacy
- Access Governance
- Artificial Intelligence
- AI Security
- Compliance
- Governance
trust_url: https://www.lightbeam.ai/trust/
---
