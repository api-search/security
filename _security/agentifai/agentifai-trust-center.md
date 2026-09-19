---
certification_count: 5
certifications:
- SOC 2 Type 2
- ISO/IEC 27001
- ISO/IEC 42001:2023
- PCI DSS v4.0.0
- HIPAA
description: ''
kind: trust-center
layout: security
name: Agentifai Trust Center
name_suffix: Trust Center
overview: AgentifAI maintains a public trust center documenting SOC 2 Type 2, ISO/IEC 27001, ISO/IEC 42001:2023, PCI DSS v4.0.0, and HIPAA compliance.
provider_name: AgentifAI
provider_slug: agentifai
slug: agentifai-trust-center
source_filename: agentifai-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: searched\nsource: https://trust.agentifai.com/\ntrust_center:\n  url: https://trust.agentifai.com/\n  platform: SafeBase by Drata\n  discovered_via: >-\n    Linked from the footer of https://www.agentifai.com/aliceos — it is not linked from the\n    homepage, and no subdomain enumeration would have found it because the host sits behind\n    Cloudflare.\n  http_status: 403\n  status_note: >-\n    A raw GET with a browser User-Agent returns a Cloudflare bot-challenge interstitial (403).\n    The page is NOT dead: a rendering fetch returns the full SafeBase trust center with named\n    certifications, document list, subprocessors and a security contact. The 403 is an ordinary\n    edge policy, recorded rather than penalised.\n  self_serve_documents: false\n  document_access: >-\n    Reports are gated behind a \"Get access\" request form; the certifications themselves are\n    listed publicly.\ncertifications:\n- name: SOC 2 Type 2\n  document:\
  \ SOC 2 Report\n  access: on-request\n- name: ISO/IEC 27001\n  document: ISO 27001 Certificate\n  access: on-request\n- name: ISO/IEC 42001:2023\n  access: listed\n- name: PCI DSS v4.0.0\n  access: listed\n- name: HIPAA\n  document: HIPAA BAA Report\n  access: on-request\nreports:\n- Penetration Test Report\n- Vulnerability Assessment Report\n- SOC 2 Report\n- ISO 27001 Certificate\n- HIPAA BAA Report\ncontrol_categories:\n- product-security\n- data-security\n- access-control\n- infrastructure\n- policies\n- legal\n- ai-governance\n- app-security\n- network-security\n- incident-response\n- business-continuity-and-disaster-recovery\nsubprocessors:\n  published: true\n  named:\n  - Atlassian\n  - Twilio\n  - Google Cloud\n  note: >-\n    Twilio and Google Cloud are consistent with the telephony and cloud posture the company\n    describes in its own llms-full.txt (SIP/CTI telephony, deployment across Azure/AWS/GCP).\nsecurity_contact:\n  published: true\n  form: email\n  value: null\n  note:\
  \ >-\n    A security contact address is displayed on the trust center but was returned obfuscated by\n    the rendering fetch. Recorded as present-but-unread rather than guessed; no address is\n    asserted here.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agentifai/refs/heads/main/security/agentifai-trust-center.yml
summary_line: SOC 2 Type 2, ISO/IEC 27001, ISO/IEC 42001:2023, PCI DSS v4.0.0, HIPAA
tags:
- Company
- Artificial Intelligence
- Conversational AI
- Voice
- Contact Center
- Banking
- Healthcare
- Agents
- Portugal
trust_url: ''
---
