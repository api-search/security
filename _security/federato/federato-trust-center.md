---
certifications: []
description: ''
kind: trust-center
layout: security
name: Federato Trust Center
name_suffix: Trust Center
overview: Federato maintains a public trust center covering its security and compliance posture.
provider_name: Federato
provider_slug: federato
slug: federato-trust-center
source_filename: federato-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nprobe: true\nsource: https://www.federato.ai/llms.txt\nurl: https://trust.federato.ai/\nprovider: vanta\n# Federato publishes a hosted Trust Center (Vanta). Existence is verified: it is\n# linked from the official marketing site and llms.txt, and the portal + its\n# sub-pages resolve. Named certifications are rendered client-side (JS) on the\n# Vanta portal and are not machine-readable from the server response, so specific\n# framework names (e.g. SOC 2 / ISO 27001) are NOT asserted here to avoid\n# fabrication. Review the portal directly for the current certification list.\ncertifications: []\npages:\n- {label: Trust Center, url: 'https://trust.federato.ai/'}\n- {label: Controls, url: 'https://trust.federato.ai/controls'}\n- {label: Resources, url: 'https://trust.federato.ai/resources'}\n- {label: Subprocessors, url: 'https://trust.federato.ai/subprocessors'}\nevidence:\n- source: https://www.federato.ai/llms.txt\n  kind: official-site-link\n\
  \  note: 'Trust Center listed under Company Information and Legal and Compliance'\n- source: https://trust.federato.ai/\n  kind: live-portal\n  note: 'Vanta-hosted trust center resolves (data-slugid present)'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/federato/refs/heads/main/security/federato-trust-center.yml
summary_line: trust center published
tags:
- Company
- Insurance Tech
- InsurTech
- Insurance
- Underwriting
- RiskOps
- Policy Lifecycle
- Artificial Intelligence
trust_url: https://trust.federato.ai/
---
