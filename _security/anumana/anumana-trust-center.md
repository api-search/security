---
certifications: []
description: ''
kind: trust-center
layout: security
name: Anumana Trust Center
name_suffix: Trust Center
overview: Anumana maintains a public trust center covering its security and compliance posture.
provider_name: Anumana
provider_slug: anumana
slug: anumana-trust-center
source_filename: anumana-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nprobe: true\nurl: https://trust.anumana.ai/\nplatform: Vanta (trust report)\ncertifications: []\ncertifications_readable: false\nx-evidence:\n  fetched: '2026-08-02'\n  url: https://trust.anumana.ai/\n  http_status: 200\n  content_type: text/html\n  content_location: https://assets.vanta.com/static/index-trust-report.bac6fdd16dd7ed43562471c5b0e3793882464477.html\n  page_title: Anumana Trust Center\n  vanta_slug_id: 0ldo9mv02uebxq0lo1djg\nnotes:\n- 'A trust center is genuinely published at trust.anumana.ai and is served by Vanta\n  (assets.vanta.com trust-report bundle, Vanta datadog application id in the page shell).'\n- 'The page is fully client-rendered and its content API requires a signed request\n  (app.vanta.com/graphql returns \"Missing `signature` or `signedAt`\"; api.vanta.com\n  trust-center endpoints return 401). No named certification (SOC 2, ISO 27001, HIPAA,\n  HITRUST, FedRAMP) could be read anonymously.'\n- 'Because no\
  \ certification names were verifiable, no `Compliance` pointer is emitted\n  in apis.yml. Recording presence without readable certifications would credit a\n  compliance posture that was not observed. Re-probe if Vanta exposes the report\n  publicly or if certifications are named on anumana.ai.'\nrelated:\n  vulnerability_disclosure: security/anumana-vulnerability-disclosure.yml\n  regulatory_conformance: conformance/anumana-conformance.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anumana/refs/heads/main/security/anumana-trust-center.yml
summary_line: trust center published
tags:
- Company
- Healthcare
- Artificial Intelligence
- Machine-Learning
- Medical Devices
- Cardiology
- Diagnostics
- Clinical Decision Support
- ECG
- Digital Health
trust_url: https://trust.anumana.ai/
---
