---
certifications:
- SOC 2 Type II
description: ''
kind: trust-center
layout: security
name: Knoetic Trust Center
name_suffix: Trust Center
overview: Knoetic maintains a public trust center documenting SOC 2 Type II compliance.
provider_name: Knoetic
provider_slug: knoetic
slug: knoetic-trust-center
source_filename: knoetic-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nprobe: true\nurl: https://trust.knoetic.com\nplatform: Vanta Trust Center\nplatform_evidence: trust.knoetic.com is a CNAME to cname.vantatrust.com; the page is the Vanta trust-report\n  application (title \"Knoetic Trust Center\", report slug mx71nqjesc0cdowcwuudd)\ncertifications:\n- SOC 2 Type II\nevidence:\n- source: https://trust.knoetic.com\n  kind: trust-center\n  detail: HTTP 200, page title \"Knoetic Trust Center\", served by Vanta (vantatrust.com CNAME)\n- source: https://cpohq.com/\n  kind: compliance-claim\n  detail: 'marketing site displays the string \"SOC 2 Type II\"'\ncaveats: >-\n  The Vanta trust report renders client-side, so the full control/document list and any additional\n  frameworks could not be enumerated without JavaScript. Only SOC 2 Type II is recorded because it is\n  the one framework named verbatim on a fetched page. Document access on Vanta trust centers is\n  typically gated behind an NDA request. Re-run\
  \ with a headless browser to enumerate the full list.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/knoetic/refs/heads/main/security/knoetic-trust-center.yml
summary_line: SOC 2 Type II
tags:
- Company
- Hr Tech
- People Analytics
- Human Resources
- Workforce Analytics
- Artificial Intelligence
- AI Agents
- SaaS
- Community
- Benchmarking
trust_url: https://trust.knoetic.com
---
