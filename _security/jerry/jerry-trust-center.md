---
certifications: []
description: ''
kind: trust-center
layout: security
name: Jerry Trust Center
name_suffix: Trust Center
overview: Jerry maintains a public trust center covering its security and compliance posture.
provider_name: Jerry
provider_slug: jerry
slug: jerry-trust-center
source_filename: jerry-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nprobe: true\nurl: https://trust.jerry.ai/\nplatform: Vanta Trust Center\nverified: true\ncertifications: []\ncertifications_note: >-\n  The trust center is confirmed live and is genuinely Jerry's — it resolves via\n  CNAME to Vanta (608b03e38041cfc516961f48.cname.vantatrust.com), carries\n  `<link rel=\"canonical\" href=\"https://trust.jerry.ai\">`, and the document title\n  is \"Jerry, Inc. Trust Center\". The page body is client-rendered by Vanta's\n  React bundle, so the served HTML is a 5.5KB shell containing no framework or\n  certification names. NO certifications are recorded here because none were\n  observed in a fetched response — recording SOC 2 / ISO 27001 without seeing\n  them would be fabrication. Named certifications require a JavaScript render or\n  an authenticated Vanta request and remain an open enrichment gap.\nevidence:\n- source: https://trust.jerry.ai/\n  http_status: 200\n  content_type: text/html\n  title: Jerry,\
  \ Inc. Trust Center\n  canonical: https://trust.jerry.ai\n  cname: 608b03e38041cfc516961f48.cname.vantatrust.com\n  vanta_slug_id: lxkt8itlc4ptbgq2lc861p\n  rendered: false\n  body_bytes: 5553\n- source: https://trust.getjerry.com/\n  dns: 608b03e38041cfc516961f48.cname.vantatrust.com\n  http_status: 0\n  note: Same Vanta CNAME target but no TLS certificate for this name; trust.jerry.ai\n    is the served hostname.\nregulatory:\n  note: >-\n    Jerry's public compliance posture is licensing rather than certification.\n    Jerry Insurance Agency, LLC is a licensed insurance producer in all 50 US\n    states and the District of Columbia; the state-by-state license register is\n    published.\n  licenses_page: https://jerry.ai/insurance-licenses/\nx-evidence:\n  fetched: '2026-08-04'\n  method: HTTP GET, no credentials, no JavaScript execution\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jerry/refs/heads/main/security/jerry-trust-center.yml
summary_line: trust center published
tags:
- Company
- Insurance
- Insurtech
- Auto Insurance
- Insurance Broker
- Automotive
- Consumer Finance
- Lending
- Telematics
- Mobile Applications
- Artificial Intelligence
trust_url: https://trust.jerry.ai/
---
