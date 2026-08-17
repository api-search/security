---
certifications: []
description: ''
kind: trust-center
layout: security
name: Lavender Trust Center
name_suffix: Trust Center
overview: Lavender maintains a public trust center covering its security and compliance posture.
provider_name: Lavender
provider_slug: lavender
slug: lavender-trust-center
source_filename: lavender-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nprobe: true\nverified: false\nurl: https://trust.lavender.ai/\nnotes: >-\n  Lavender has provisioned a Drata-hosted trust center at trust.lavender.ai — the\n  hostname CNAMEs to trust.cname.drata.com, which is Drata's trust-center hosting\n  target and is a deliberate act of configuration by the company, not an accident of\n  the platform. However the page itself could NOT be read: every request returns HTTP\n  403 behind a Cloudflare interstitial (\"Just a moment...\", challenges.cloudflare.com),\n  including with a browser User-Agent, and Drata's public API paths return 403/401.\n  Because the document was never actually retrieved, no certifications are recorded\n  from it and NO `TrustCenter` pointer is wired into apis.yml. Presence of a DNS\n  record is not the same as a served, readable trust center, and this pipeline does\n  not award a pointer for a surface it has not read. Lavender's published compliance\n  claims (SOC 2 Type\
  \ 2, GDPR, CCPA) come from the privacy page instead and are\n  captured in conformance/lavender-conformance.yml, which is what the existing\n  `Compliance` pointer refers to.\ncertifications: []\ncertifications_note: >-\n  None readable from the trust center. See conformance/lavender-conformance.yml for\n  the compliance claims Lavender publishes in readable form.\nevidence:\n- source: dns\n  record: CNAME\n  name: trust.lavender.ai\n  value: trust.cname.drata.com.\n  observed: '2026-08-13'\n- source: https://trust.lavender.ai/\n  http_status: 403\n  reason: Cloudflare bot challenge interstitial\n  observed: '2026-08-13'\n- source: https://trust.lavender.ai/robots.txt\n  http_status: 403\n  observed: '2026-08-13'\n- source: https://public-api.drata.com/trust/lavender\n  http_status: 401\n  observed: '2026-08-13'\nto_confirm: >-\n  A human browser session (or an allow-listed fetch) against https://trust.lavender.ai/\n  would confirm the trust center and its certification list; on confirmation,\
  \ set\n  verified: true, populate certifications[], and add a `type: TrustCenter` pointer.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lavender/refs/heads/main/security/lavender-trust-center.yml
summary_line: trust center published
tags:
- Company
- Sales
- Email
- Artificial Intelligence
- Sales Enablement
- Sales Engagement
- CRM
- Browser Extension
- Productivity
trust_url: https://trust.lavender.ai/
---
