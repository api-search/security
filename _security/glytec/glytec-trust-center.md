---
certifications:
- HITRUST CSF
- HIPAA
- FDA 510(k) clearance (Class II Software as a Medical Device)
description: ''
kind: trust-center
layout: security
name: Glytec Trust Center
name_suffix: Trust Center
overview: Glytec maintains a public trust center documenting HITRUST CSF, HIPAA, and FDA 510(k) clearance (Class II Software as a Medical Device) compliance.
provider_name: Glytec
provider_slug: glytec
slug: glytec-trust-center
source_filename: glytec-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: searched\nprobe: true\nurl: https://trust.glytec.com/\nplatform: SafeBase\naccess: gated\nnotes: >-\n  trust.glytec.com is a live Glytec-owned hostname that 301-redirects to a SafeBase trust portal\n  (https://app.safebase.io/portal/8299b4b1-9453-4990-8635-127021c41ec4/preview). The portal itself is\n  behind SafeBase authentication (302 to auth.safebase.io/authorize), so the document set — SOC reports,\n  policies, subprocessor list — could not be enumerated anonymously. The certifications recorded below\n  come from Glytec's own PUBLIC security and compliance page, not from the gated portal.\ncertifications:\n- HITRUST CSF\n- HIPAA\n- FDA 510(k) clearance (Class II Software as a Medical Device)\npublic_compliance_page: https://glytec.com/glytec-one-platform/security-and-compliance/\nclaims:\n- claim: HIPAA\n  quote: >-\n    GlytecOne's full platform architecture is designed and maintained in compliance with HIPAA requirements.\n  source: https://glytec.com/glytec-one-platform/security-and-compliance/\n\
  - claim: HITRUST CSF certified\n  quote: >-\n    HITRUST CSF certification validates that GlytecOne meets the rigorous information security and risk\n    management requirements.\n  source: https://glytec.com/glytec-one-platform/security-and-compliance/\n- claim: FDA-cleared Class II Software as a Medical Device\n  quote: >-\n    Glucommander is an FDA-cleared Class II Software as a Medical Device (SaMD), subject to ongoing quality\n    system requirements, post-market surveillance, and device change controls.\n  source: https://glytec.com/glytec-one-platform/security-and-compliance/\nnot_found:\n- SOC 2 (not named on the public compliance page)\n- ISO 27001 (not named on the public compliance page)\n- PCI DSS (not applicable / not named)\n- FedRAMP (not named)\n- Published penetration-test summary\n- Named security contact or responsible-disclosure policy\nevidence:\n- source: https://trust.glytec.com/\n  http_status: 301\n  redirects_to: https://app.safebase.io/portal/8299b4b1-9453-4990-8635-127021c41ec4/preview?product=default\n\
  \  observed: '2026-08-04'\n- source: https://glytec.com/glytec-one-platform/security-and-compliance/\n  http_status: 200\n  keywords: [hipaa, hitrust csf, fda-cleared, samd, cloud-based]\n  observed: '2026-08-04'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/glytec/refs/heads/main/security/glytec-trust-center.yml
summary_line: HITRUST CSF, HIPAA, FDA 510(k) clearance (Class II Software as a Medical Device)
tags:
- Company
- Healthcare
- Health IT
- Clinical Decision Support
- Diabetes
- Insulin Management
- glycemic-management
- Hospital
- EHR Integration
- HL7
- Medical Device
- Software as a Medical Device
trust_url: https://trust.glytec.com/
---
