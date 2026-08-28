---
certifications:
- HITRUST
- HIPAA Business Associate Agreement (BAA)
description: Sempre Health runs a hosted trust center at trust.semprehealth.com, built on Vanta. The page was fetched successfully (HTTP 200) and is genuinely Sempre Health's - <link rel="canonical" href="https://trust.semprehealth.com">, <title>Sempre Health Trust Center</title>, and a description naming Sempre Health's prescription savings product. The certification list itself is rendered client-side from Vanta's GraphQL API, which rejects anonymous reads (POST https://app.vanta.com/graphql -> HTTP 400 "Missing `signature` or `signedAt`"), so the documents and control list published inside the trust center could not be enumerated without a browser session. The one certification Sempre Health names in plain text on its own site is HITRUST.
kind: trust-center
layout: security
name: Sempre Health Trust Center
name_suffix: Trust Center
overview: Sempre Health maintains a public trust center documenting HITRUST and HIPAA Business Associate Agreement (BAA) compliance.
provider_name: Sempre Health
provider_slug: sempre-health
slug: sempre-health-trust-center
source_filename: sempre-health-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: searched\nsource: https://trust.semprehealth.com/\nname: Sempre Health Trust Center\ndescription: 'Sempre Health runs a hosted trust center at trust.semprehealth.com,\n  built on Vanta. The page was fetched successfully (HTTP 200) and is genuinely Sempre\n  Health''s - <link rel=\"canonical\" href=\"https://trust.semprehealth.com\">, <title>Sempre\n  Health Trust Center</title>, and a description naming Sempre Health''s prescription\n  savings product. The certification list itself is rendered client-side from Vanta''s\n  GraphQL API, which rejects anonymous reads (POST https://app.vanta.com/graphql ->\n  HTTP 400 \"Missing `signature` or `signedAt`\"), so the documents and control list\n  published inside the trust center could not be enumerated without a browser session.\n  The one certification Sempre Health names in plain text on its own site is HITRUST.'\ntrust_center:\n  url: https://trust.semprehealth.com/\n  platform: Vanta\n  status:\
  \ live\n  http_status: 200\n  content_type: text/html\n  machine_readable: false\n  note: Vanta trust-report SPA; contents load from a signed GraphQL endpoint and are\n    not anonymously enumerable.\ncertifications:\n- name: HITRUST\n  evidence: https://www.semprehealth.com/health-plans/\n  quote: Sempre signs a BAA & MSA and is HITRUST certified.\n  method: searched\n- name: HIPAA Business Associate Agreement (BAA)\n  evidence: https://www.semprehealth.com/health-plans/\n  quote: Sempre signs a BAA & MSA and is HITRUST certified.\n  method: searched\nnot_found:\n  - No SOC 2, ISO 27001, PCI DSS or FedRAMP claim is made anywhere on the public site.\n  - No security.txt, /security page, or public bug bounty could be found (see security/sempre-health-vulnerability-disclosure.yml).\nx-evidence:\n- url: https://trust.semprehealth.com/\n  status: 200\n  fetched: '2026-08-26'\n- url: https://www.semprehealth.com/health-plans/\n  status: 200\n  fetched: '2026-08-26'\n- url: https://app.vanta.com/graphql\n\
  \  status: 400\n  fetched: '2026-08-26'\n  note: anonymous introspection rejected - \"Missing `signature` or `signedAt`\"\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sempre-health/refs/heads/main/security/sempre-health-trust-center.yml
summary_line: HITRUST, HIPAA Business Associate Agreement (BAA)
tags:
- Company
- Health
- Healthcare
- Digital Health
- Pharmacy
- Pharmacy Benefits
- Prescriptions
- Medication Adherence
- Patient Engagement
- Health Plans
- SMS
trust_url: ''
---
