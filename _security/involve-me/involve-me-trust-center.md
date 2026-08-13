---
certifications:
- SOC 2 Type II
- GDPR
description: involve.me operates a real trust centre on its own subdomain, hosted by Vanta (EU tenant, app.eu.vanta.com). Its certification list is client-rendered and is therefore NOT readable from the served HTML, so the certifications recorded below are taken from involve.me's own first-party blog announcement rather than scraped from the trust centre itself.
kind: trust-center
layout: security
name: Involve Me Trust Center
name_suffix: Trust Center
overview: involve.me maintains a public trust center documenting SOC 2 Type II and GDPR compliance.
provider_name: involve.me
provider_slug: involve-me
slug: involve-me-trust-center
source_filename: involve-me-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: >-\n  https://trust.involve.me/ (HTTP 200, a Vanta-hosted trust report) and\n  https://www.involve.me/blog/soc2-compliance (HTTP 200, involve.me's own SOC 2\n  Type II announcement dated 2026-07-01).\nurl: https://trust.involve.me/\ndescription: >-\n  involve.me operates a real trust centre on its own subdomain, hosted by Vanta\n  (EU tenant, app.eu.vanta.com). Its certification list is client-rendered and is\n  therefore NOT readable from the served HTML, so the certifications recorded below\n  are taken from involve.me's own first-party blog announcement rather than scraped\n  from the trust centre itself.\n\nprovider: Vanta\ntenant_region: EU (app.eu.vanta.com)\nmachine_readable: false\nmachine_readable_note: >-\n  The served HTML is a 7.4 KB SPA shell; the trust report is assembled client-side\n  from assets.vanta.com bundles. No JSON endpoint, feed or server-rendered fallback\n  was found, so an agent visiting trust.involve.me\
  \ learns nothing.\n\ncertifications:\n- name: SOC 2 Type II\n  status: attested\n  date: '2026-07-01'\n  auditor: not published\n  report_access: >-\n    Under NDA, to Enterprise-plan customers or prospects with a signed engagement\n    letter; requested through the trust centre.\n  evidence: https://www.involve.me/blog/soc2-compliance\n- name: GDPR\n  status: compliance claimed\n  evidence: https://www.involve.me/blog/soc2-compliance\n  supporting:\n  - https://www.involve.me/data-processing\n  - https://www.involve.me/privacy\n  note: >-\n    stereosense GmbH is EU-domiciled (https://www.involve.me/imprint) and webhook\n    deliveries originate from AWS eu-central-1, so EU data residency is consistent\n    with the claim.\n\nnot_claimed:\n- ISO 27001\n- ISO 27701\n- HIPAA\n- FedRAMP\n- PCI DSS\nnot_claimed_note: >-\n  None of these appears in any first-party source found. They are recorded as\n  not-claimed rather than absent, because the trust centre's own framework list\n  could not\
  \ be read.\n\nevidence:\n- url: https://trust.involve.me/\n  http_status: 200\n  content_type: text/html\n  observation: >-\n    og:title \"involve.me Trust Center\"; Vanta signature manifest and\n    index-trust-report bundle preloaded; no certification names in the served body.\n- url: https://www.involve.me/blog/soc2-compliance\n  http_status: 200\n  observation: >-\n    First-party announcement of SOC 2 Type II, explicitly contrasting Type II with\n    Type I, confirming GDPR compliance, and linking trust.involve.me for report access.\n\nx-correction:\n  date: '2026-08-12'\n  note: >-\n    This file replaces an automated probe result that was a FALSE POSITIVE. The\n    probe followed https://security.involve.me, which 302s into involve.me's own\n    funnel-hosting edge and lands on the MARKETING HOMEPAGE with\n    utm_campaign=customer_organization-deleted. The keyword matcher then found\n    \"soc 2\" and \"gdpr\" in that homepage's copy and recorded the redirected\n    marketing\
  \ URL as a trust centre. security.involve.me is not a trust centre and\n    serves no security content; the real one is trust.involve.me.\n  bad_source: >-\n    https://www.involve.me/?utm_source=involveme&utm_medium=referral&utm_campaign=customer_organization-deleted&utm_content=security&utm_term=https%3A%2F%2Fsecurity.involve.me\n  bad_source_status: 200 (after a 302 from https://security.involve.me)\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/involve-me/refs/heads/main/security/involve-me-trust-center.yml
summary_line: SOC 2 Type II, GDPR
tags:
- Company
- Marketing
- Lead Generation
- Forms
- Surveys
- Quizzes
- No-Code
- Email Marketing
- CRM
- Webhooks
- Model Context Protocol
- Austria
trust_url: https://trust.involve.me/
---
