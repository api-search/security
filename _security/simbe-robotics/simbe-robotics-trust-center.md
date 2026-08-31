---
certifications: []
description: ''
kind: trust-center
layout: security
name: Simbe Robotics Trust Center
name_suffix: Trust Center
overview: Simbe Robotics maintains a public trust center covering its security and compliance posture.
provider_name: Simbe Robotics
provider_slug: simbe-robotics
slug: simbe-robotics-trust-center
source_filename: simbe-robotics-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: probed\nsource: https://trust.simberobotics.com/\nnote: >-\n  Simbe operates a Vanta-hosted trust center at trust.simberobotics.com. It resolves via\n  CNAME to cname.vantatrust.com and serves the Vanta trust-report application (title\n  \"Simbe Trust Center\", assets under assets.vanta.com/static/index-trust-report-*). The trust\n  center EXISTS and is publicly reachable, but its contents are rendered client-side: the served\n  HTML is a 5,441-byte shell that carries no certification names, so the certification list could\n  not be read without executing JavaScript. NO certifications are asserted here and NO Compliance\n  pointer is emitted in apis.yml, because naming a framework we did not actually observe would be\n  fabrication. This is a provider-fixable gap: server-render the framework list, or publish it on a\n  crawlable page.\ntrust_center:\n  present: true\n  url: https://trust.simberobotics.com/\n  http_status: 200\n  platform: Vanta\n\
  \  hosted: true\n  cname: 65878918ea18d7882cd68889.cname.vantatrust.com\n  machine_readable: false\n  rendering: client-side single-page application\ncertifications: []\ncertifications_note: >-\n  Not readable from the served HTML. Unverified — do not infer SOC 2 / ISO 27001 from the presence\n  of a Vanta trust center.\ndocuments:\n- label: Gated document request\n  url: https://app.vanta.com/doc?s=yyac825qosl5vp5fw0el1e\n  note: >-\n    A Vanta document link is present on the trust center. Vanta document links of this shape\n    typically require an access request or NDA acceptance; not fetched.\nsubprocessors_published: unknown\nsecurity_contact_published: false\nsecurity_contact_note: >-\n  No /.well-known/security.txt on any Simbe host, and no security or vulnerability-disclosure page\n  found on www.simberobotics.com (/security -> 404, /legal -> 404). No Security pointer is emitted.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/simbe-robotics/refs/heads/main/security/simbe-robotics-trust-center.yml
summary_line: trust center published
tags:
- Company
- Robotics
- Retail
- Inventory
- Computer-Vision
- Artificial Intelligence
- Store Intelligence
- RFID
- Supply Chain
- Physical AI
trust_url: ''
---
