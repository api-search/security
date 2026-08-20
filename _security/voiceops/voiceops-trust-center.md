---
certifications:
- SOC 2
- HIPAA
- PCI DSS
description: ''
kind: trust-center
layout: security
name: Voiceops Trust Center
name_suffix: Trust Center
overview: VoiceOps maintains a public trust center documenting SOC 2, HIPAA, and PCI DSS compliance.
provider_name: VoiceOps
provider_slug: voiceops
slug: voiceops-trust-center
source_filename: voiceops-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nprobe: true\nurl: https://trust.voiceops.com/\nplatform: vanta\ncertifications:\n  - SOC 2\n  - HIPAA\n  - PCI DSS\ncertifications_source: >-\n  Named on the VoiceOps homepage (https://www.voiceops.com/), in the data\n  section: \"Your data stays yours. SOC 2 · HIPAA · PCI DSS. We never use it to\n  train AI.\" These are the company's own published claims. They were NOT read\n  off the trust center itself — see notes — and no certificate, audit report,\n  attestation letter or report date is publicly downloadable, so the level\n  (e.g. SOC 2 Type I vs Type II) and the audit window are unknown.\nnotes: >-\n  Verified live (HTTP 200) Vanta-hosted trust center titled \"Voiceops Trust\n  Center\" (slugid g5bubu9n88g5aq1mcqumiv), with a /controls sub-page. The\n  framework and control lists are rendered client-side behind Vanta's signed\n  queries and still could not be extracted without a browser on this round, so\n  the certification\
  \ list above is taken from the homepage rather than the trust\n  center. Note also that every /.well-known/* path on trust.voiceops.com returns\n  HTTP 200 with the Vanta SPA HTML shell; that is a catch-all, not a served\n  document, and is explicitly not counted anywhere in this profile. Do not\n  confuse this company with voiceops.io, a different company.\nevidence:\n  - source: https://trust.voiceops.com/\n    kind: trust-center\n    http_status: 200\n    detail: 'Vanta trust-report app (assets.vanta.com bundle, slugid g5bubu9n88g5aq1mcqumiv); meta description confirms compliance artifacts and controls'\n  - source: https://trust.voiceops.com/controls\n    kind: trust-center-controls\n    http_status: 200\n    detail: 'Controls page reachable; body is client-side rendered and yielded only the page title to a non-browser fetch'\n  - source: https://www.voiceops.com/\n    kind: homepage-compliance-claim\n    http_status: 200\n    detail: 'Homepage text: \"Your data stays yours. SOC 2\
  \ · HIPAA · PCI DSS. We never use it to train AI.\"'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/voiceops/refs/heads/main/security/voiceops-trust-center.yml
summary_line: SOC 2, HIPAA, PCI DSS
tags:
- Company
- Ai Apps
- Conversation Intelligence
- Call Centers
- Sales Coaching
- Customer Experience
- Artificial Intelligence
- Speech Analytics
- MCP
- Agents
trust_url: https://trust.voiceops.com/
---
