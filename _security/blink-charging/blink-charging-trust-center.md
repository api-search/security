---
certifications: []
description: 'Verbatim page description: "Our Trust Center provides transparency into Blink Charging''s information security and compliance program. Here, you can review our security controls, compliance posture, and supporting documentation."'
kind: trust-center
layout: security
name: Blink Charging Trust Center
name_suffix: Trust Center
overview: Blink Charging maintains a public trust center covering its security and compliance posture.
provider_name: Blink Charging
provider_slug: blink-charging
slug: blink-charging-trust-center
source_filename: blink-charging-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: searched\nprobe: true\nsource: live probe 2026-07-27 (DNS + HTTPS)\nurl: https://trust.blinkcharging.com\ntitle: Blink Charging Trust Center\nplatform: Vanta\nverified: true\ncertifications: []\ncertifications_readable: false\ndescription: >-\n  Verbatim page description: \"Our Trust Center provides transparency into Blink Charging's\n  information security and compliance program. Here, you can review our security controls,\n  compliance posture, and supporting documentation.\"\nevidence:\n- source: dns\n  detail: >-\n    trust.blinkcharging.com CNAMEs to 68bf19561bc8f4c48cb2adba.cname.vantatrust.com\n    (104.18.26.175, 104.18.27.175) - a Vanta-hosted trust centre on the company's own domain.\n- source: https://trust.blinkcharging.com/\n  detail: >-\n    HTTP 200, 3,751-byte Vanta SPA shell, <title>Blink Charging Trust Center</title>, canonical\n    https://trust.blinkcharging.com, og:image https://app.vanta.com/doc?s=jn9lvhu6v4k5q8oj2msfka\n\
  \    (a real 18KB JPEG card), slugid x6v528vlr1uan8vnkr20r.\n- source: https://trust.blinkcharging.com/graphql\n  detail: >-\n    POST {\"query\":\"{__typename}\"} returns HTTP 400\n    {\"errors\":[{\"message\":\"Missing `signature` or `signedAt`\",\"extensions\":{\"code\":\"BAD_REQUEST\"}}]}\n    - Vanta requires a signed request, so the control/certification list is not readable\n    anonymously and NO certification is recorded here. Named certs would require loading the page\n    in a browser or requesting documents through Vanta's access flow.\nnotes: >-\n  This is the only security-programme surface Blink publishes. It is NOT linked from\n  blinkcharging.com navigation or any of the 985 sitemap URLs - it was found by hostname probe.\n  Nothing on the marketing site names a certification; the one named programme there is FedRAMP\n  \"In Process\" (2024-06-13). See conformance/blink-charging-conformance.yml.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blink-charging/refs/heads/main/security/blink-charging-trust-center.yml
summary_line: trust center published
tags:
- Energy
- United States
- EV Charging
- Electric Vehicles
- Charging Stations
- Grid
- Demand Response
- Fleet Management
- OCPP
- OpenADR
- Roaming
trust_url: https://trust.blinkcharging.com
---
