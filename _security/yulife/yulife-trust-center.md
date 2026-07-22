---
certifications: []
description: ''
kind: trust-center
layout: security
name: Yulife Trust Center
name_suffix: Trust Center
overview: Yulife maintains a public trust center covering its security and compliance posture.
provider_name: Yulife
provider_slug: yulife
slug: yulife-trust-center
source_filename: yulife-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nprobe: true\nurl: https://trust.yulife.com/\nplatform: Vanta\ncertifications: []\nnotes: >-\n  YuLife operates a Vanta-hosted Trust Center at https://trust.yulife.com/.\n  Existence verified via the response content-location header pointing at a\n  Vanta trust-report asset. The specific named frameworks/certifications and\n  documents are served behind Vanta's authenticated report API and could not be\n  read verbatim, so none are asserted here (no fabrication). Refresh by\n  requesting access to the trust report to enumerate SOC 2 / ISO 27001 / etc.\nevidence:\n- source: https://trust.yulife.com/\n  kind: vanta-trust-center\n  signal: content-location https://assets.vanta.com/static/index-trust-report...html\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yulife/refs/heads/main/security/yulife-trust-center.yml
summary_line: trust center published
tags:
- Company
- Insurtech
- Insurance
- Employee Benefits
- Wellbeing
- Group Life Insurance
- Health Insurance
- B Corp
trust_url: https://trust.yulife.com/
---
