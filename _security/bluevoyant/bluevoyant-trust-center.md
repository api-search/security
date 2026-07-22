---
certifications: []
description: ''
kind: trust-center
layout: security
name: Bluevoyant Trust Center
name_suffix: Trust Center
overview: Bluevoyant maintains a public trust center covering its security and compliance posture.
provider_name: Bluevoyant
provider_slug: bluevoyant
slug: bluevoyant-trust-center
source_filename: bluevoyant-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nprobe: true\nsource: live probe of trust.bluevoyant.com + DNS CNAME\nurl: https://trust.bluevoyant.com/\nprovider: Vanta\n# Verified a genuine trust center exists: trust.bluevoyant.com is a CNAME to\n# 68e52645927d8f7f1f2e48d2.cname.vantatrust.com and returns HTTP 200 with the\n# page title \"BlueVoyant Trust Center\". The report content is rendered by a\n# Vanta client-side SPA, so specific named certifications could not be\n# enumerated verbatim from the page body and are intentionally left empty\n# rather than fabricated. Populate certifications[] on a future pass that can\n# read the Vanta trust-report data.\ncertifications: []\nevidence:\n- source: dns\n  kind: cname\n  value: 68e52645927d8f7f1f2e48d2.cname.vantatrust.com\n- source: https://trust.bluevoyant.com/\n  kind: http\n  status: 200\n  title: BlueVoyant Trust Center\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bluevoyant/refs/heads/main/security/bluevoyant-trust-center.yml
summary_line: trust center published
tags:
- Company
- Cybersecurity
- Managed Detection and Response
- Threat Intelligence
- Supply Chain Security
- Digital Risk Protection
- Security Operations
trust_url: https://trust.bluevoyant.com/
---
