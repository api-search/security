---
certification_count: 1
certifications:
- SOC 2
description: ''
kind: trust-center
layout: security
name: Wellfound Trust Center
name_suffix: Trust Center
overview: Wellfound maintains a public trust center documenting SOC 2 compliance.
provider_name: Wellfound
provider_slug: wellfound
slug: wellfound-trust-center
source_filename: wellfound-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: searched\nsource: >-\n  https://trust.wellfound.ai/ (200) and\n  https://help.wellfound.com/article/1213-wellfound-ai-ats-connection-what-we-access-why-we-need-it-and-what-we-do-with-your-data\n  (200)\ntrust_center:\n  url: https://trust.wellfound.ai/\n  http_status: 200\n  title: Wellfound Trust Center\n  platform: Vanta\n  platform_evidence: >-\n    The page is served from Vanta's trust-center product - assets load from\n    assets.vanta.com, the document carries data-slugid=\"kwb5hos99yzvm26qd1ykhz\" and the\n    og:image resolves to https://app.vanta.com/doc?s=wwsuwhttugmuxiis1iz8j4.\n  domain_note: >-\n    The trust center lives on wellfound.ai, not wellfound.com. This is Wellfound's own second\n    brand - wellfound.ai / cloud.wellfound.com both redirect into reach.wellfound.com, the\n    Wellfound Reach application - and the trust center is linked from Wellfound's own help\n    center, so the different domain is confirmed first-party\
  \ rather than a third party's page.\n  readable_by_machine: false\n  readable_note: >-\n    The page renders entirely client-side; every /.well-known/* path on the host returns the\n    same 5,436-byte HTML shell. Certifications, subprocessors and report metadata are behind\n    the JS render and, in Vanta's product, usually behind an NDA request as well, so the\n    document list could not be enumerated by probe.\ncertifications:\n- name: SOC 2\n  status: claimed\n  verified_by_probe: false\n  evidence: >-\n    \"Both Wellfound and Merge (our ATS integration provider) are SOC 2 compliant.\" -\n    https://help.wellfound.com/article/1213-wellfound-ai-ats-connection-what-we-access-why-we-need-it-and-what-we-do-with-your-data\n  type: not stated (Type I vs Type II not published)\n  period: not stated\nsubprocessors:\n- name: Merge\n  role: ATS integration provider (unified API broker for Greenhouse, Lever, Ashby, Workable,\n    Gem and others)\n  url: https://www.merge.dev/\n  security_page:\
  \ https://www.merge.dev/security\n  soc2_claimed: true\n  evidence: same help-center article; Wellfound names Merge as a subprocessor in its own words\n    (\"subprocessors such as Merge\").\n- name: Atlassian Statuspage\n  role: status page (status.wellfound.com)\n  evidence: page footer \"Powered by Atlassian Statuspage\"; the host serves Atlassian's own\n    security.txt.\n- name: Vanta\n  role: trust center hosting (trust.wellfound.ai)\n- name: Cloudflare\n  role: CDN, WAF and bot mitigation in front of every Wellfound host probed\n- name: SendGrid\n  role: transactional email (named as a monitored component on status.wellfound.com)\n- name: Iterable\n  role: marketing/lifecycle email (named as a monitored component on status.wellfound.com)\n- name: AWS\n  role: hosting, us-west-2 (named as monitored components on status.wellfound.com)\nsecurity_contact:\n  email: security@wellfound.com\n  source: https://wellfound.com/.well-known/security.txt\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wellfound/refs/heads/main/security/wellfound-trust-center.yml
summary_line: SOC 2
tags:
- Recruiting
- Hiring
- Talent
- Human Resources
- Applicant Tracking
- Job Board
- Startups
- MCP
- agent-native
- OAuth
- AI Sourcing
trust_url: ''
---
