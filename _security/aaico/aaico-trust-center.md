---
api_specs:
- filename: postman-collection
  format: yaml
  label: Opus Platform API
  slug: opus-platform-api
  spec_type: Postman
  url: https://developer.opus.com/api-reference/v0-jobs/postman-collection
certification_count: 6
certifications:
- SOC 2 Type II
- ISO 27001
- ISO 42001
- HIPAA
- GDPR
- EU AI Act
description: ''
kind: trust-center
layout: security
name: Aaico Trust Center
name_suffix: Trust Center
overview: AppliedAI (AAICO) maintains a public trust center documenting SOC 2 Type II, ISO 27001, ISO 42001, HIPAA, GDPR, and EU AI Act compliance.
provider_name: AppliedAI (AAICO)
provider_slug: aaico
slug: aaico-trust-center
source_filename: aaico-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: searched\nsource: https://trust.opus.com/\nurl: https://trust.opus.com/\nname: Opus Trust Center\nplatform: Vanta (EU tenant)\nx-evidence:\n  fetched: '2026-09-05'\n  url: https://trust.opus.com/\n  http_status: 200\n  content_type: text/html\n  title: Opus Trust Center\n  meta_description: Trust, Security, Compliance, Automation\n  vanta_document_reference: https://app.eu.vanta.com/doc?s=ftiu9wqamqqyrz2eo2n2\nnote: >-\n  A live, first-party trust center exists and is hosted on Vanta's EU tenant under AAICO's own\n  opus.com domain. The page body is fully client-rendered — the served HTML is a 5.5KB Vanta\n  bootstrap shell — so the certification list, subprocessors and controls cannot be read without\n  executing JavaScript, and the backing data endpoints return the same shell rather than JSON.\n  The certifications recorded below were therefore read from AAICO's own enterprise page, which\n  names them in plain text, NOT scraped from the trust\
  \ center.\ncertifications:\n- name: SOC 2 Type II\n  source: https://www.opus.com/enterprise\n- name: ISO 27001\n  source: https://www.opus.com/enterprise\n- name: ISO 42001\n  source: https://www.opus.com/enterprise\n- name: HIPAA\n  source: https://www.opus.com/enterprise\n- name: GDPR\n  source: https://www.opus.com/enterprise\n- name: EU AI Act\n  source: https://www.opus.com/enterprise\ndocuments:\n- name: Opus Data Processing Agreement\n  url: https://www.opus.com/legal-docs/Opus-DPA.pdf\n  status: 200\n- name: Opus Support Service Standards\n  url: https://www.opus.com/legal-docs/Opus-Support-Service-Standards.pdf\n  status: 200\nreport_access: gated — audit reports are requested through the Vanta trust center, not downloadable anonymously\ngaps:\n- Trust center content is JS-only; no machine-readable certification list is served.\n- No security.txt on any host, so there is no RFC 9116 route to a security contact.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aaico/refs/heads/main/security/aaico-trust-center.yml
summary_line: SOC 2 Type II, ISO 27001, ISO 42001, HIPAA, GDPR, EU AI Act
tags:
- Company
- Artificial Intelligence
- Workflow Automation
- Agents
- Enterprise
- Document Processing
- Regulated Industries
- Business Process Automation
- Banking
- Insurance
- Healthcare
- Model Context Protocol
trust_url: https://trust.opus.com/
---
