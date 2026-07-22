---
certifications: []
description: ''
kind: trust-center
layout: security
name: Linx Security Trust Center
name_suffix: Trust Center
overview: Linx Security maintains a public trust center covering its security and compliance posture.
provider_name: Linx Security
provider_slug: linx-security
slug: linx-security-trust-center
source_filename: linx-security-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nprobe: true\nurl: https://trust.linx.security\nstatus: 200\nnotes: >-\n  A dedicated Trust Center exists at trust.linx.security and returns HTTP 200,\n  but it is a client-rendered single-page app (a 545-byte HTML shell that boots\n  a JS bundle) whose <title> is \"Trust Center\". No certifications are present in\n  the served HTML, and the app has no unauthenticated JSON API — probed\n  /api/config, /api/trust-center, /api/v1/config and /api/v1/trust-center all\n  return the SPA catch-all rather than data. The automated probe\n  (probe-security-programs.py) therefore scored this trust=none; this file is\n  the hand-verified record that the trust center is real. Certifications below\n  come ONLY from the compliance badges published in the linx.security site\n  footer, not from the trust center itself, and are marked with their source\n  accordingly. No SOC 2 / ISO 27001 report or attestation letter was retrievable\n  without authentication,\
  \ so none is asserted.\ncertifications_verified: []\ncertifications_claimed:\n- name: HIPAA\n  source: https://www.linx.security\n  evidence: footer compliance badge (alt=\"HIPAA\")\n  confidence: badge-only\n- name: AICPA\n  source: https://www.linx.security\n  evidence: footer compliance badge (alt=\"AICPA\")\n  confidence: badge-only\n  note: >-\n    The AICPA badge is the conventional marker for a SOC 2 examination, but the\n    footer does not state SOC 2 Type I vs Type II and no report was retrievable,\n    so SOC 2 is NOT asserted as a verified certification here.\nother_badges:\n- Fortune Cyber 60 2020\n- Duns 100\n- AWS\n- Azure\naccess:\n  self_service: false\n  note: Report access appears to require a request/NDA flow inside the trust center app.\nevidence:\n- source: https://trust.linx.security\n  kind: trust-center\n  status: 200\n  rendered: false\n- source: https://www.linx.security\n  kind: footer-compliance-badges\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/linx-security/refs/heads/main/security/linx-security-trust-center.yml
summary_line: trust center published
tags:
- Company
- Security
- Identity
- Identity Governance
- Access Management
- Identity Security
- Non-Human Identity
- Agentic AI
- MCP
- IGA
trust_url: https://trust.linx.security
---
