---
certifications: []
description: ''
kind: trust-center
layout: security
name: Dispatchhealth Trust Center
name_suffix: Trust Center
overview: DispatchHealth maintains a public trust center covering its security and compliance posture.
provider_name: DispatchHealth
provider_slug: dispatchhealth
slug: dispatchhealth-trust-center
source_filename: dispatchhealth-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-07-31'\nmethod: probed\nprobe: true\nurl: https://trust.dispatchhealth.com/\nprovider: Drata\ncertifications: []\nverified: dns-delegation\nevidence:\n- source: dig CNAME trust.dispatchhealth.com\n  observed: trust.cname.drata.com.\n  kind: dns-delegation-to-trust-center-host\n  note: the provider has delegated trust.dispatchhealth.com to Drata's hosted trust-center\n    service, which is direct evidence of a published trust center\n- source: https://trust.dispatchhealth.com/\n  http_status: 403\n  content_type: text/html; charset=UTF-8\n  kind: http-probe\n  note: 'Cloudflare interstitial (\"Just a moment...\") returned to both curl and the\n    fetch tool; the page body could not be read, so the certifications listed on the\n    trust center could NOT be enumerated in this pass. certifications[] is deliberately\n    empty rather than guessed.'\nx-evidence:\n  fetched: '2026-07-31'\n  url: https://trust.dispatchhealth.com/\n  http_status: 403\n  content_type:\
  \ text/html; charset=UTF-8\n  dns_cname: trust.cname.drata.com.\nnotes: 'No Compliance pointer was emitted: the trust center exists but no named certification\n  (SOC 2 / ISO 27001 / HITRUST / HIPAA attestation) could be verified from a first-party\n  source in this pass. Re-run when the page is readable to enumerate certifications\n  and upgrade to method: searched.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dispatchhealth/refs/heads/main/security/dispatchhealth-trust-center.yml
summary_line: trust center published
tags:
- Company
- Healthcare
- Health Systems
- Hospital at Home
- Home Health
- Urgent Care
- Care Delivery
- Medical Services
- Telehealth
- Digital Health
trust_url: https://trust.dispatchhealth.com/
---
