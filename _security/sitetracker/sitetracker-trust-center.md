---
certifications:
- SOC 1 Type II
- SOC 2 Type II
- ISO/IEC 27001
- ISO/IEC 27701
description: ''
kind: trust-center
layout: security
name: Sitetracker Trust Center
name_suffix: Trust Center
overview: Sitetracker maintains a public trust center documenting SOC 1 Type II, SOC 2 Type II, ISO/IEC 27001, and ISO/IEC 27701 compliance.
provider_name: Sitetracker
provider_slug: sitetracker
slug: sitetracker-trust-center
source_filename: sitetracker-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: searched\nsource: >-\n  https://www.sitetracker.com/legal/ (links the trust center);\n  https://trust.sitetracker.com/ (live, Cloudflare bot challenge);\n  https://www.sitetracker.com/products-services/integrations/ (certification names)\nnote: >-\n  Sitetracker runs a real, dedicated trust center. It is hosted by Drata\n  (trust.sitetracker.com CNAMEs to trust.cname.drata.com) and is linked from\n  https://www.sitetracker.com/legal/ and https://www.sitetracker.com/trust/,\n  which 302s to it. Our probe could not read the page body: every request\n  returns HTTP 403 with `cf-mitigated: challenge`, a Cloudflare bot challenge —\n  the page demonstrably exists and only our crawler was turned away, so this is\n  recorded as present-but-unread, not as absent. The certifications below are\n  therefore taken from Sitetracker's own public integrations page rather than\n  from the trust center itself.\ntrust_center:\n  url: https://trust.sitetracker.com/\n\
  \  platform: Drata\n  platform_evidence: 'DNS: trust.sitetracker.com CNAME trust.cname.drata.com'\n  linked_from:\n  - https://www.sitetracker.com/legal/\n  - https://www.sitetracker.com/trust/\n  reachable: false\n  http_status: 403\n  unreadable_reason: \"Cloudflare bot challenge (cf-mitigated: challenge)\"\ncertifications:\n- name: SOC 1 Type II\n  source: https://www.sitetracker.com/products-services/integrations/\n- name: SOC 2 Type II\n  source: https://www.sitetracker.com/products-services/integrations/\n- name: ISO/IEC 27001\n  source: https://www.sitetracker.com/products-services/integrations/\n- name: ISO/IEC 27701\n  source: https://www.sitetracker.com/products-services/integrations/\nrelated_documents:\n- name: Subprocessors\n  url: https://www.sitetracker.com/subprocessors/\n  status: 200\n- name: Privacy Policy\n  url: https://www.sitetracker.com/privacy-policy/\n  status: 200\n- name: Master Services Agreement\n  url: https://www.sitetracker.com/legal-msa/\n  status: 200\n\
  evidence:\n- url: https://trust.sitetracker.com/\n  status: 403\n- url: https://www.sitetracker.com/trust/\n  status: 403\n- url: https://www.sitetracker.com/legal/\n  status: 200\n- url: https://www.sitetracker.com/products-services/integrations/\n  status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sitetracker/refs/heads/main/security/sitetracker-trust-center.yml
summary_line: SOC 1 Type II, SOC 2 Type II, ISO/IEC 27001, ISO/IEC 27701
tags:
- Company
- Telecommunications
- Utilities
- Energy
- EV Charging
- Fiber Networks
- Asset Management
- Project Management
- Field Service
- Salesforce
- Critical Infrastructure
trust_url: ''
---
