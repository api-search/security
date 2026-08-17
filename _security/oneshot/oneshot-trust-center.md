---
certifications: []
description: ''
kind: trust-center
layout: security
name: Oneshot Trust Center
name_suffix: Trust Center
overview: OneShot maintains a public trust center covering its security and compliance posture.
provider_name: OneShot
provider_slug: oneshot
slug: oneshot-trust-center
source_filename: oneshot-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nprobe: true\nsource: https://security.oneshot.ai\nurl: https://security.oneshot.ai\nplatform: Vanta\ntitle: OneShot.ai Trust Center\ncertifications: []\nnote: >-\n  OneShot operates a branded Vanta Trust Center at https://security.oneshot.ai. The host\n  is verified first-party by DNS: it CNAMEs to 66589c2f3a3cc20954b0df68.cname.vantatrust.com,\n  Vanta's trust-center delegation target, and the served document carries\n  <title>OneShot.ai Trust Center</title> with <link rel=\"canonical\" href=\"https://security.oneshot.ai\">.\n  This is a real trust center, not the SPA false positive — the host exists only for this purpose.\n  NO CERTIFICATIONS ARE RECORDED because none are publicly readable: the trust-center content is\n  rendered client-side from a signed-operation GraphQL API, so the served HTML (4,530 bytes)\n  contains no framework or certification names, and Vanta trust centers gate document access\n  behind an access request.\
  \ certifications: [] means \"checked, nothing publicly readable\",\n  not \"none held\". A future pass should re-check if OneShot enables the public overview.\nevidence:\n- source: https://security.oneshot.ai\n  http_status: 200\n  content_type: text/html\n  signal: title \"OneShot.ai Trust Center\"; canonical https://security.oneshot.ai\n- source: dns\n  record: security.oneshot.ai CNAME 66589c2f3a3cc20954b0df68.cname.vantatrust.com\n  signal: dedicated Vanta trust-center delegation\nrelated:\n- type: gdpr-commitment\n  url: https://www.oneshot.ai/handlingdata\n- type: data-processing-terms\n  url: https://www.oneshot.ai/data-processing\n- type: privacy-policy\n  url: https://www.oneshot.ai/privacy-policy\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oneshot/refs/heads/main/security/oneshot-trust-center.yml
summary_line: trust center published
tags:
- Company
- Sales
- Sales Automation
- Outbound
- Prospecting
- Lead Generation
- Artificial Intelligence
- Go-To-Market
trust_url: https://security.oneshot.ai
---
