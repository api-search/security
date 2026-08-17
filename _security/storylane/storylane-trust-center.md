---
api_specs:
- filename: storylane-connect
  format: yaml
  label: Storylane External API
  slug: storylane-external-api
  spec_type: Postman
  url: https://www.postman.com/team-storylane/storylane-public/collection/2zkg7jc/storylane-connect
certifications:
- SOC 2 Type 2
- GDPR
description: 'Storylane operates a public Trust Center hosted on Sprinto at trust.storylane.io, carrying a SOC 2 Type 2 report, a penetration test report, an EU/UK Data Processing Agreement, a subprocessor list and a live control register. It is the company''s only structured security-and-compliance surface — there is no security.txt and no vulnerability disclosure program anywhere on the estate.

  '
kind: trust-center
layout: security
name: Storylane Trust Center
name_suffix: Trust Center
overview: Storylane maintains a public trust center documenting SOC 2 Type 2 and GDPR compliance.
provider_name: Storylane
provider_slug: storylane
slug: storylane-trust-center
source_filename: storylane-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nprobe: true\nsource: https://trust.storylane.io/\nurl: https://trust.storylane.io/\ndescription: >\n  Storylane operates a public Trust Center hosted on Sprinto at\n  trust.storylane.io, carrying a SOC 2 Type 2 report, a penetration test report,\n  an EU/UK Data Processing Agreement, a subprocessor list and a live control\n  register. It is the company's only structured security-and-compliance surface —\n  there is no security.txt and no vulnerability disclosure program anywhere on\n  the estate.\nplatform: Sprinto\nverified: probed\nhttp_status: 200\nprobe_note: >\n  IMPORTANT PROBE CAVEAT. trust.storylane.io sits behind CloudFront with a WAF\n  rule that returns HTTP 403 \"Request blocked\" to non-browser user agents. A\n  default curl request reports 403; the same URL returns 200 with a browser\n  User-Agent. Any automated check that does not set a browser UA will record this\n  live trust center as unavailable.\ncertifications:\n\
  \  - name: SOC 2 Type 2\n    year: '2026'\n    document: Storylane Inc - SOC 2 Type 2 - Final Report.pdf\n    access: gated (request via the Trust Center, NDA flow)\n    evidence: SOC 2 framework badge and the named final report listed on trust.storylane.io\n  - name: GDPR\n    document: EU and UK Personal Data Processing Agreement 1.2.5.5.pdf\n    access: published on the Trust Center\n    evidence: >\n      \"Storylane is GDPR compliant and our DPA is available in the Storylane\n      Trust Center\" — https://docs.storylane.io/trust-and-security/gdpr-compliance\ndocuments_listed:\n  - name: Storylane Inc - SOC 2 Type 2 - Final Report.pdf\n    type: audit report\n  - name: Storylane INC Security-Scan-Report.pdf\n    type: penetration / security scan report\n  - name: EU and UK Personal Data Processing Agreement 1.2.5.5.pdf\n    type: data processing agreement\n  - name: Subprocessor list\n    type: subprocessors\ncontrols_published:\n  note: >\n    The Sprinto trust center exposes a live\
  \ control register with per-control\n    pass state. Controls observed by name include:\n  observed:\n    - Vulnerability Remediation Process\n    - Centralized Management of Flaw Remediation Processes\n    - Application security practices (unauthorized access and modification)\nnot_found:\n  - name: ISO 27001\n    checked: true\n    result: not listed\n  - name: HIPAA\n    checked: true\n    result: not listed\n  - name: PCI DSS\n    checked: true\n    result: not listed\n  - name: FedRAMP\n    checked: true\n    result: not listed\nrelated:\n  gdpr_docs: https://docs.storylane.io/trust-and-security/gdpr-compliance\n  sso_docs: https://docs.storylane.io/trust-and-security/sso\n  privacy_contact: privacy@storylane.io\n  domain_security: security/storylane-domain-security.yml\ngaps:\n  - No security.txt on any host (RFC 9116 absent).\n  - No vulnerability disclosure or bug bounty program (HackerOne 404, Bugcrowd 404, no disclosure page).\n  - No published security contact address; support@storylane.io\
  \ and privacy@storylane.io are the only channels.\n  - The SOC 2 report is gated behind a request flow rather than summarized publicly.\nevidence:\n  - source: https://trust.storylane.io/\n    http_status: 200\n    user_agent: browser\n    keywords:\n      - SOC 2 Type 2\n      - SOC 2 - 2026\n      - GDPR\n      - Subprocessor\n      - Pentest\n      - DPA\n      - Vulnerability Remediation Process\n  - source: https://trust.storylane.io/\n    http_status: 403\n    user_agent: default (curl)\n    note: CloudFront WAF blocks non-browser agents\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/storylane/refs/heads/main/security/storylane-trust-center.yml
summary_line: SOC 2 Type 2, GDPR
tags:
- Interactive Demos
- Product Walkthroughs
- Sales Enablement
- Marketing
- Demo Analytics
- Demo Automation
- Buyer Hub
- Sales
- MCP
- Agent Tools
- Webhooks
- Embeds
- oEmbed
- Demo Automation Platform
trust_url: https://trust.storylane.io/
---
