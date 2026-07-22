---
certifications: []
description: ''
kind: trust-center
layout: security
name: Artian Trust Center
name_suffix: Trust Center
overview: Artian maintains a public trust center covering its security and compliance posture.
provider_name: Artian
provider_slug: artian
slug: artian-trust-center
source_filename: artian-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nprobe: true\nurl: https://trust.artian.ai/\nplatform: Vanta\nverified: true\ncertifications: []\nevidence:\n- source: https://trust.artian.ai/\n  kind: vanta-trust-center\n  detail: >-\n    Returns a Vanta trust-report application shell with data-slugid\n    \"ke34u0ivnjslzyfic3myy\" and data-environment \"prod\". Confirmed not to be wildcard\n    DNS - control subdomains (zzznotreal.artian.ai, randomxyz123.artian.ai) fail to\n    resolve, so this host is deliberately provisioned.\n- source: https://artian.ai/\n  kind: site-link\n  detail: The Artian homepage links out to https://trust.artian.ai\nnotes: >-\n  The trust center is real and reachable, but Vanta renders its report contents\n  client-side and the Vanta report API (api.vanta.com) returns \"Unauthorized\" for\n  anonymous requests, so no named certification could be read from public fetches.\n  `certifications` is deliberately left empty rather than guessed, and no\n  `Compliance`\
  \ pointer is wired in apis.yml. A render-capable (headless-browser) pass\n  should revisit this to extract SOC 2 / ISO 27001 status and upgrade the artifact.\nautomated_probe_result:\n  script: 0-working/probe-security-programs.py\n  trust: none\n  reason: >-\n    The probe requires two or more trust/compliance keywords in the response body;\n    the Vanta shell contains no server-rendered text, so the probe correctly did not\n    record a hit. This artifact was written from manual verification instead.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/artian/refs/heads/main/security/artian-trust-center.yml
summary_line: trust center published
tags:
- Company
- Artificial Intelligence
- AI Agents
- Agentic AI
- Financial Services
- Enterprise Software
- Workflow Automation
- AI Governance
- Model Risk Management
- Insurance
trust_url: https://trust.artian.ai/
---
