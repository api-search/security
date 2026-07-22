---
certifications: []
description: ''
kind: trust-center
layout: security
name: Tessl Trust Center
name_suffix: Trust Center
overview: Tessl maintains a public trust center covering its security and compliance posture.
provider_name: Tessl
provider_slug: tessl
slug: tessl-trust-center
source_filename: tessl-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nprobe: true\nurl: https://trust.tessl.io/\nsource: https://www.tessl.io/\n# Tessl links a dedicated Trust Center (trust.tessl.io, HTTP 200) from its\n# marketing site. The certification list is rendered client-side (JS) and could\n# not be verified verbatim by fetch/probe on this pass, so no specific\n# certifications are asserted here and no `Compliance` pointer is emitted.\n# Re-run to capture named certs (SOC 2 / ISO 27001 / GDPR) once the page is\n# server-rendered or via the trust-center vendor API.\ncertifications: []\ncertifications_verified: false\nsecurity_contact: security@tessl.io\nnotes: >-\n  Trust Center exists and is publicly linked; Snyk-powered security scanning is a\n  first-class platform feature (skill/plugin install policies gate on critical/high\n  Snyk findings). Named compliance certifications were not machine-verifiable on\n  this pass.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tessl/refs/heads/main/security/tessl-trust-center.yml
summary_line: trust center published
tags:
- Company
- Ai
- Agents
- Agentic Development
- Developer Tools
- Agent Skills
- MCP
- CLI
- Registry
- Code Review
trust_url: https://trust.tessl.io/
---
