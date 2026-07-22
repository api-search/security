---
certifications: []
description: ''
kind: trust-center
layout: security
name: Levocred Ai Trust Center
name_suffix: Trust Center
overview: Levocred AI maintains a public trust center covering its security and compliance posture.
provider_name: Levocred AI
provider_slug: levocred-ai
slug: levocred-ai-trust-center
source_filename: levocred-ai-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nprobe: true\nurl: https://trust.levocred.com/\nplatform: Oneleet\nstatus: 200\ncertifications: []\ncertifications_note: >-\n  The trust center is live and hosted on Oneleet (trust.levocred.com is a CNAME to\n  trust.oneleet.com). Its contents are rendered client-side, so no named certification\n  (SOC 2, ISO 27001, PCI DSS, HIPAA, FedRAMP) could be verified from the served HTML.\n  Certifications are deliberately left empty rather than assumed, and no Compliance\n  pointer is wired in apis.yml. Re-probe with a rendering fetch to populate.\nevidence:\n- source: dns\n  detail: trust.levocred.com CNAME -> trust.oneleet.com\n- source: https://trust.levocred.com/\n  detail: HTTP 200, document title \"Trust center\", Oneleet-hosted single-page app\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/levocred-ai/refs/heads/main/security/levocred-ai-trust-center.yml
summary_line: trust center published
tags:
- Company
- Artificial Intelligence
- Financial Services
- Private Credit
- Lending
- Credit Risk
- Fintech
- Y Combinator
trust_url: https://trust.levocred.com/
---
