---
api_specs:
- filename: callrail-accounts-api-openapi.yml
  format: yaml
  label: CallRail Accounts API
  slug: callrail-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/callrail/refs/heads/main/openapi/callrail-accounts-api-openapi.yml
- filename: callrail-calls-api-openapi.yml
  format: yaml
  label: CallRail Calls API
  slug: callrail-calls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/callrail/refs/heads/main/openapi/callrail-calls-api-openapi.yml
certifications:
- ISO 42001
- SOC 2 Type II
- HIPAA/HITECH
- PCI
- GDPR
- CCPA
description: CallRail runs a Conveyor-hosted Trust Center at trust.callrail.com and a public Security & Compliance page at callrail.com/security that names each certification and links a PDF or certificate for it.
kind: trust-center
layout: security
name: Callrail Trust Center
name_suffix: Trust Center
overview: CallRail maintains a public trust center documenting ISO 42001, SOC 2 Type II, HIPAA/HITECH, PCI, GDPR, and CCPA compliance.
provider_name: CallRail
provider_slug: callrail
slug: callrail-trust-center
source_filename: callrail-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nprobe: true\nsource: https://trust.callrail.com/\nurl: https://trust.callrail.com/\ncompliance_page: https://www.callrail.com/security\ndescription: >-\n  CallRail runs a Conveyor-hosted Trust Center at trust.callrail.com and a public\n  Security & Compliance page at callrail.com/security that names each certification and links a\n  PDF or certificate for it.\ncertifications:\n  - name: ISO 42001\n    detail: >-\n      International standard for AI Management Systems. CallRail states it is the first in the lead\n      intelligence industry to achieve it.\n    evidence_url: https://cdn.mediavalet.com/usva/callrail/5G5pOJO060Kj1FZFrhaqqw/Qs9xhIoxu0KoZiSB23qBdg/Original/CallRail%20-%20ISO%2042001-2023%20Certificate.pdf\n  - name: SOC 2 Type II\n    detail: AICPA Service Organization Control 2, Type II.\n    evidence_url: https://www.callrail.com/usva/callrail/8ixJQwzZlkuBizzhSK09kA/jUgxdIpx0USV27Zbp84xkw/Original/SOC_2_compliance.pdf\n\
  \  - name: HIPAA/HITECH\n    detail: >-\n      End-to-end solution for health care providers and the agencies serving them; the v3 API\n      exposes a `hipaa_account` flag on the account object and a HIPAA-specific variant of the call\n      recording endpoint.\n    evidence_url: https://www.callrail.com/usva/callrail/4g3exyu5k0GqpErYVw2qpg/AEcW9ddKukqZCoAeoBAFrQ/Original/HIPAA_compliance.pdf\n  - name: PCI\n    detail: PII redaction feature to reduce liability when payment information is spoken on a recorded or transcribed call.\n    evidence_url: https://www.callrail.com/usva/callrail/pkVFEXTZgEyFhuY16rOBtA/G3wN0kTl3k6mHn34DeWtzw/Original/PCI.pdf\n  - name: GDPR\n    detail: EU General Data Protection Regulation posture.\n    evidence_url: https://www.callrail.com/usva/callrail/23FeJHMNREant2JpS7j7PA/hSMAt6h8BkigopJUkJ7-0g/Original/GDPR.pdf\n  - name: CCPA\n    detail: California Consumer Privacy Act posture.\n    evidence_url: https://www.callrail.com/usva/callrail/3YcDpEmtd0u5mvzzU18CTA/dfkiXN7acU6c28AU_GKZBQ/Original/CCPA.pdf\n\
  responsible_ai:\n  url: https://www.callrail.com/security/ai\n  note: Published AI principles page (transparency, ethical innovation, security), tied to the ISO 42001 certification.\nvulnerability_disclosure:\n  url: https://www.callrail.com/security/disclosure\n  detail: security/callrail-vulnerability-disclosure.yml\nsubprocessors:\n  published: true\n  count: 12\n  source: https://trust.callrail.com/\n  last_updated: '2026-02-03'\nevidence:\n  - source: https://www.callrail.com/security\n    http_status: 200\n    fetched: '2026-08-14'\n    keywords: [ISO 42001, SOC 2 (Type II), HIPAA/HITECH, PCI, GDPR, CCPA, Vulnerability Disclosure Program]\n  - source: https://trust.callrail.com/\n    http_status: 200\n    fetched: '2026-08-14'\n    keywords: [trust center, soc2-type-2, iso-42001, hipaa, pci]\nx-corrections:\n  - date: '2026-08-14'\n    note: >-\n      Replaced the certification list written by probe-security-programs.py on the same day, which\n      recorded SOC 2, ISO 27001, ISO\
  \ 27017, ISO 27018, HIPAA, FedRAMP and GDPR. Those were FALSE\n      POSITIVES: trust.callrail.com is a Conveyor trust center whose page payload embeds the\n      certification arrays of OTHER vendors (CallRail's subprocessors — Salesforce, AWS, Zendesk\n      and others), and the keyword scan picked them up. CallRail's own certification array in that\n      same payload is [\"hipaa\",\"soc2-type-2\",\"pci\",\"iso-42001\"], which matches its public\n      Security & Compliance page exactly. CallRail holds no ISO 27001/27017/27018 and no FedRAMP\n      authorization that it publishes.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/callrail/refs/heads/main/security/callrail-trust-center.yml
summary_line: ISO 42001, SOC 2 Type II, HIPAA/HITECH, PCI, GDPR, CCPA
tags:
- Call Tracking
- Conversation Intelligence
- Marketing Attribution
- Lead Tracking
- Telephony
- Analytics
- Form Tracking
trust_url: https://trust.callrail.com/
---
