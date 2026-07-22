---
certifications: []
description: ''
kind: trust-center
layout: security
name: Ben Trust Center
name_suffix: Trust Center
overview: Ben maintains a public trust center covering its security and compliance posture.
provider_name: Ben
provider_slug: ben
slug: ben-trust-center
source_filename: ben-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nprobe: true\nurl: https://trust.thanksben.com/\nplatform: Vanta\n# Ben publishes a Vanta-hosted Trust Center. The page returns HTTP 200 and is a\n# genuine trust/compliance surface (meta keywords: Trust, Security, Compliance).\n# Named certifications are served client-side via the gated Vanta trust-report API\n# (api.vanta.com returned 401 without a viewer NDA/access grant), so specific\n# framework names (e.g. SOC 2 / ISO 27001) could not be verified from the public\n# surface and are NOT asserted here — no fabrication. Request access via the page\n# to see the underlying reports.\ncertifications: []\nevidence:\n- source: https://trust.thanksben.com/\n  status: 200\n  keywords: [trust, security, compliance]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ben/refs/heads/main/security/ben-trust-center.yml
summary_line: trust center published
tags:
- Company
- Employee Benefits
- Human Resources
- HR Tech
- Rewards and Recognition
- Global Benefits
- Employee Experience
- Compliance
trust_url: https://trust.thanksben.com/
---
