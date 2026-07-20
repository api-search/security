---
certifications:
- SOC 2 Type II
- GDPR
description: ''
kind: trust-center
layout: security
name: Brownie Trust Center
name_suffix: Trust Center
overview: IncidentFox (Brownie) maintains a public trust center documenting SOC 2 Type II and GDPR compliance.
provider_name: IncidentFox (Brownie)
provider_slug: brownie
slug: brownie-trust-center
source_filename: brownie-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nprobe: true\nsource: https://docs.incidentfox.ai/security\nurl: https://docs.incidentfox.ai/security\ncertifications:\n- SOC 2 Type II\n- GDPR\nposture:\n- Envoy-based credentials proxy - secrets never touch the agent; dynamic credential injection at request time\n- Claude SDK SRE agent runs in isolated Kubernetes sandboxes with gVisor user-space kernel isolation\n- Egress-restricted network policies (HTTPS/443 only) and bounded CPU/memory/time resource limits\n- Ephemeral sandboxes destroyed after each investigation\n- Full audit trail of agent actions; human approval gates on all write operations\nevidence:\n- source: https://docs.incidentfox.ai/security\n  keywords:\n  - soc 2 type ii\n  - compliance certification\n- source: https://incidentfox.ai/sub-processors.html\n  keywords:\n  - soc 2\n  - gdpr\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brownie/refs/heads/main/security/brownie-trust-center.yml
summary_line: SOC 2 Type II, GDPR
tags:
- Company
- Incident Response
- SRE
- AIOps
- Observability
- DevOps
- Artificial Intelligence
- Developer Tools
- Automation
- Open Source
trust_url: https://docs.incidentfox.ai/security
---
