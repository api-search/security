---
certifications:
- SOC 2 Type 2
- ISO/IEC 27001:2022
- CMMC Level 2
- CSA STAR Level 1
- NIST SP 800-171
- GDPR
- CCPA
- HECVAT Lite
description: ''
kind: trust-center
layout: security
name: Simspace Trust Center
name_suffix: Trust Center
overview: SimSpace maintains a public trust center documenting SOC 2 Type 2, ISO/IEC 27001:2022, CMMC Level 2, CSA STAR Level 1, NIST SP 800-171, GDPR, CCPA, and HECVAT Lite compliance.
provider_name: SimSpace
provider_slug: simspace
slug: simspace-trust-center
source_filename: simspace-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: searched\nsource: https://trust.simspace.com/\nurl: https://trust.simspace.com/\nhost: SafeBase by Drata\nnote: >-\n  trust.simspace.com sits behind a Cloudflare interstitial to a plain curl (HTTP 403,\n  \"Just a moment...\"), but the page demonstrably exists and renders to a browser\n  user-agent — it is a bot challenge, not a dead pointer. Certifications below were\n  read from the rendered page.\ncertifications:\n- id: soc2-type2\n  name: SOC 2 Type 2\n- id: iso-27001-2022\n  name: ISO/IEC 27001:2022\n- id: cmmc-level-2\n  name: CMMC Level 2\n  note: Validated against NIST SP 800-171.\n- id: csa-star-level-1\n  name: CSA STAR Level 1\n- id: nist-800-171\n  name: NIST SP 800-171\n- id: gdpr\n  name: GDPR\n- id: ccpa\n  name: CCPA\n- id: hecvat-lite\n  name: HECVAT Lite\ndocuments_gated: true\ndocuments_note: SafeBase trust centers gate the underlying reports (SOC 2 report, ISO\n  certificate) behind an NDA request form; only the badge list\
  \ is public.\nvulnerability_disclosure:\n  published_policy: false\n  note: >-\n    The trust center exposes SafeBase's generic \"Report issue\" control, but SimSpace\n    publishes no named vulnerability disclosure or responsible disclosure policy, no\n    bug bounty program (no HackerOne, Bugcrowd or Intigriti listing was found), and no\n    /.well-known/security.txt (404 on simspace.com and api.simspace.com). No\n    Security / VulnerabilityDisclosure pointer is emitted for that reason.\nx-evidence:\n- url: https://trust.simspace.com/\n  http_status: 403\n  note: Cloudflare bot challenge to curl; page renders for a browser user-agent.\n  fetched: '2026-08-27'\n- url: https://simspace.com/.well-known/security.txt\n  http_status: 404\n  fetched: '2026-08-27'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/simspace/refs/heads/main/security/simspace-trust-center.yml
summary_line: SOC 2 Type 2, ISO/IEC 27001:2022, CMMC Level 2, CSA STAR Level 1, NIST SP 800-171, GDPR, CCPA, HECVAT Lite
tags:
- Company
- Cybersecurity
- Cyber Range
- Security Training
- Simulation
- AI Agents
- Security Operations
- Critical Infrastructure
- Government
- Compliance
trust_url: https://trust.simspace.com/
---
