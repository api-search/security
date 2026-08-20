---
certifications:
- ISO/IEC 27001
- SOC 2
- GDPR
description: ''
kind: trust-center
layout: security
name: Caretta Trust Center
name_suffix: Trust Center
overview: Caretta maintains a public trust center documenting ISO/IEC 27001, SOC 2, and GDPR compliance.
provider_name: Caretta
provider_slug: caretta
slug: caretta-trust-center
source_filename: caretta-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nprobe: true\nurl: https://trust.caretta.so\nhttp_status: 200\n\nvendor: Oneleet\nvendor_evidence: >-\n  trust.caretta.so is a CNAME to trust.oneleet.com (resolved 2026-08-13), the\n  hosted trust-center product.\n\ncertifications:\n- name: ISO/IEC 27001\n  source: https://www.caretta.so\n  verified: false\n- name: SOC 2\n  source: https://www.caretta.so\n  verified: false\n- name: GDPR\n  source: https://www.caretta.so\n  verified: false\n\nverification_note: >-\n  The certifications above are claimed on Caretta's own marketing site, which\n  states \"ISO 27001 certified\", \"SOC 2 compliant\", \"GDPR compliant\" and\n  \"Enterprise-grade encryption\". They could NOT be confirmed from the trust\n  center itself: https://trust.caretta.so returns a 604-byte client-rendered\n  React shell (an empty #root div plus a bundled JS module) with no server-side\n  content, so the certification list, report availability, audit dates and\n  subprocessor\
  \ list are unreadable without executing JavaScript. Each entry is\n  therefore recorded as claimed-by-provider, unverified-by-probe. Nothing about\n  audit scope, report type (SOC 2 Type I vs Type II) or currency is asserted\n  because none of it was observable.\n\nsecurity_claims:\n- claim: Enterprise-grade encryption\n  source: https://www.caretta.so\n  specificity: low\n  note: No cipher suites, key management or encryption-at-rest detail published.\n\nvulnerability_disclosure:\n  published: false\n  security_txt: false\n  bug_bounty: null\n  contact: null\n  note: >-\n    No security.txt on caretta.so, www.caretta.so or gateway.caretta.app (all\n    404). No /security, /responsible-disclosure or /vulnerability-disclosure\n    page (404). No HackerOne, Bugcrowd or Intigriti program found, and no\n    security@ address published. Because nothing was verified, no\n    security/caretta-vulnerability-disclosure.yml artifact and no\n    type: Security pointer are emitted.\n\ndata_handling_documented:\n\
  - surface: MCP\n  claim: >-\n    The server follows the signed-in user's existing Caretta access and cannot\n    return calls the user could not otherwise see; per-client scope consent and\n    per-client revocation.\n  source: https://www.caretta.so/docs/caretta-mcp\n- surface: Zoom\n  claim: >-\n    Single Zoom permission requested (meeting:write:meeting). Caretta states it\n    does not request permission to read the Zoom profile, list existing\n    meetings, access recordings, read transcripts, or join meetings.\n  source: https://www.caretta.so/docs/zoom\n- surface: webhooks\n  claim: >-\n    Per-endpoint signing secret shown once, rotatable, with immediate\n    invalidation of the previous secret.\n  source: https://www.caretta.so/docs/webhooks\n\nevidence:\n- {source: 'https://trust.caretta.so', http_status: 200, kind: trust-center, note: 'JS-rendered SPA; no readable content'}\n- {source: 'https://www.caretta.so', http_status: 200, kind: marketing-claims, keywords: ['iso 27001',\
  \ 'soc 2', 'gdpr', 'enterprise-grade encryption']}\n- {source: 'https://www.caretta.so/.well-known/security.txt', http_status: 404, kind: negative-probe}\n- {source: 'https://www.caretta.so/security', http_status: 404, kind: negative-probe}\nfetched: '2026-08-13'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/caretta/refs/heads/main/security/caretta-trust-center.yml
summary_line: ISO/IEC 27001, SOC 2, GDPR
tags:
- Company
- Artificial Intelligence
- Sales
- Sales Intelligence
- Real-Time
- Conversation Intelligence
- Revenue Operations
- Y Combinator
- MCP
- Webhook
- Agents
trust_url: https://trust.caretta.so
---
