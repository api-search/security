---
certifications: []
description: ''
kind: trust-center
layout: security
name: Insurf Trust Center
name_suffix: Trust Center
overview: Insurf maintains a public trust center covering its security and compliance posture.
provider_name: Insurf
provider_slug: insurf
slug: insurf-trust-center
source_filename: insurf-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nprobe: true\nsource: https://www.insurf.io/security\nurl: https://www.insurf.io/security\n# The /security page is a public trust surface, but Insurf EXPLICITLY DISCLAIMS\n# certification. Per the page: \"No SOC 2 report has been issued yet. Current work\n# is readiness and evidence collection.\" and \"Insurf does not claim SOC 2\n# certification... does not claim HIPAA certification; HIPAA readiness depends on\n# BAAs, policies, and launch controls.\" SOC 2 / HIPAA are recorded below as\n# in-progress readiness ONLY, not achieved certifications. No Compliance pointer\n# is emitted because no compliance program has been published/attained.\ncertifications: []\nreadiness:\n- program: SOC 2\n  status: in-progress\n  note: No SOC 2 report issued; readiness and evidence collection via Vanta.\n- program: HIPAA\n  status: in-progress\n  note: HIPAA readiness pending BAAs, policies, and launch controls; not certified.\ncontrols:\n- Vanta monitors\
  \ Google Workspace and GitHub evidence.\n- MFA-oriented founder/admin access reviewed for production paths.\n- AWS (S3, KMS, Textract, logging) is the intended covered cloud boundary.\n- PHI vendor path limited to AWS, Vercel, Neon, and OpenAI absent a signed customer agreement.\nboundaries:\n- Does not claim SOC 2 certification or a completed SOC 2 report.\n- Does not claim HIPAA certification.\n- Public demos use synthetic or redacted material, not production PHI.\nevidence:\n- source: https://www.insurf.io/security\n  keywords:\n  - trust\n  - security\n  - soc 2 (readiness)\n  - hipaa (readiness)\n  - vanta\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/insurf/refs/heads/main/security/insurf-trust-center.yml
summary_line: trust center published
tags:
- Company
- Healthcare
- Health Insurance
- Prior Authorization
- Denial Appeals
- Revenue Cycle Management
- Insurance
- Artificial Intelligence
- Y Combinator
trust_url: https://www.insurf.io/security
---
