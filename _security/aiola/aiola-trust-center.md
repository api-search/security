---
certification_count: 2
certifications:
- SOC 2 Type II
- ISO 27001:2022
description: ''
kind: trust-center
layout: security
name: Aiola Trust Center
name_suffix: Trust Center
overview: aiOla maintains a public trust center documenting SOC 2 Type II and ISO 27001:2022 compliance.
provider_name: aiOla
provider_slug: aiola
slug: aiola-trust-center
source_filename: aiola-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-09-14'\nmethod: probed\nsource: >-\n  https://trust.aiola.ai/ — page data read from\n  https://api.scytale.ai/views/trust-center/public/page-data with the Origin and\n  Referer of trust.aiola.ai\nurl: https://trust.aiola.ai/\nplatform: Scytale\ncompany_id: 6537d4843226c50012b677c9\nraw: security/aiola-trust-center-page-data.json\nnote: >-\n  trust.aiola.ai serves a single-page-app shell with no crawlable text; the certification\n  state below is read from the public page-data document the app itself loads, so it is\n  what a visitor to the Trust Center sees rather than a marketing claim.\ncertifications:\n- name: SOC 2 Type II\n  framework: soc2-type2\n  status: fully-implemented\n  report_available: true\n  report_name: aiOla SOC2 Report 2026\n  access: request via the Trust Center\n- name: ISO 27001:2022\n  framework: iso27001-2022\n  status: fully-implemented\n  report_available: true\n  reports:\n  - 'aiOla - ISO27001:2022 Certification (One Pager)'\n \
  \ - 'aiOla - ISO27001:2022 Certification Report'\n  access: request via the Trust Center\nin_progress:\n- name: GDPR\n  framework: gdpr-2024\n  status: in-progress\n- name: CCPA 2024\n  framework: ccpa\n  status: in-progress\nsubprocessors:\n- Apollo.io\n- AWS\n- Cloudflare\n- HubSpot\n- Lemlist\n- LiveKit\n- OpenRouter\n- Salesforce\n- Snowflake\n- Twilio\nsubprocessor_note: >-\n  Published in the Trust Center's vendor list. LiveKit and OpenRouter are the two worth\n  a buyer's attention — they place real-time media transport and third-party model\n  routing inside the data path of a speech product.\ndocuments_gated: true\ndocuments_gated_note: >-\n  All three audit artifacts are behind a Trust Center access request. Framework status\n  and the subprocessor list are public; the reports are not.\nbadges_on_marketing_site:\n- SOC 2\n- ISO 27001\n- GDPR\n- CCPA\nbadge_note: >-\n  aiola.ai displays all four badges in its footer trust strip, including GDPR and CCPA,\n  which the company's\
  \ own Trust Center records as in-progress rather than implemented.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aiola/refs/heads/main/security/aiola-trust-center.yml
summary_line: SOC 2 Type II, ISO 27001:2022
tags:
- Speech Recognition
- Speech-to-Text
- Text-to-Speech
- Voice AI
- Conversational AI
- Artificial Intelligence
- Machine Learning
- Audio
- Transcription
- Enterprise
trust_url: https://trust.aiola.ai/
---
