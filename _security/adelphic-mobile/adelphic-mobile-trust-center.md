---
certifications:
- SOC 2 Type I
description: ''
kind: trust-center
layout: security
name: Adelphic Mobile Trust Center
name_suffix: Trust Center
overview: Adelphic Mobile * maintains a public trust center documenting SOC 2 Type I compliance.
provider_name: Adelphic Mobile *
provider_slug: adelphic-mobile
slug: adelphic-mobile-trust-center
source_filename: adelphic-mobile-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nprobe: true\nurl: https://trust.viantinc.com/\nplatform: UpGuard Trust Center\nownership_note: >-\n  Adelphic is Viant Technology's DSP (acquired 2017) and publishes no separate\n  trust surface; trust.viantinc.com is the trust center Viant's own security\n  page links to for the SOC 2 report covering the platform Adelphic runs on.\ncertifications:\n- SOC 2 Type I\nattestations:\n- id: soc2-type-1\n  name: SOC 2 Type I\n  framework: AICPA SSAE 18\n  statement: >-\n    \"Viant's control environment is assessed under the SOC 2 framework,\n    performed in accordance with the AICPA's Statement on Standards for\n    Attestation Engagements No. 18, or SSAE 18.\"\n  report_access: >-\n    Report is not published openly — \"For access to our SOC 2 Report please\n    refer to our trust center\" (request-gated behind the UpGuard trust center).\n  source: https://www.viantinc.com/company/security/\nregulatory_posture:\n- id: sox\n  name: Sarbanes-Oxley\
  \ (SOX)\n  note: 'Referenced as an applicable regime (Viant is a public company, NASDAQ: DSP).'\n- id: ccpa\n  name: California Consumer Privacy Act\n  note: Referenced on the security page and the privacy center.\n- id: gdpr\n  name: GDPR\n  note: >-\n    Addressed through the Viant privacy center and the Ad Platform Privacy\n    Policy; no certification is claimed.\nprivacy_center: https://www.viantinc.com/privacy-center/\nnot_claimed:\n- ISO 27001\n- PCI DSS\n- HIPAA\n- FedRAMP\n- CSA STAR\n- SOC 2 Type II\nevidence:\n- source: https://trust.viantinc.com/\n  http_status: 200\n  keywords:\n  - trust center\n  note: >-\n    The trust center itself is a client-rendered UpGuard SPA (1,083-byte HTML\n    shell); the named certification above is read from Viant's own\n    server-rendered security page, not inferred from the shell.\n- source: https://www.viantinc.com/company/security/\n  http_status: 200\n  keywords:\n  - soc 2\n  - ssae 18\n  - trust center\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adelphic-mobile/refs/heads/main/security/adelphic-mobile-trust-center.yml
summary_line: SOC 2 Type I
tags:
- Company
- Enterprise
- Advertising
- AdTech
- Programmatic Advertising
- Demand-Side Platform
- DSP
- Marketing
- Connected TV
trust_url: https://trust.viantinc.com/
---
