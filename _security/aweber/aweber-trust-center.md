---
api_specs:
- filename: aweber-accounts-api-openapi.yml
  format: yaml
  label: AWeber Accounts API
  slug: aweber-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aweber/refs/heads/main/openapi/aweber-accounts-api-openapi.yml
- filename: aweber-broadcasts-api-openapi.yml
  format: yaml
  label: AWeber Broadcasts API
  slug: aweber-broadcasts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aweber/refs/heads/main/openapi/aweber-broadcasts-api-openapi.yml
- filename: aweber-campaigns-api-openapi.yml
  format: yaml
  label: AWeber Campaigns API
  slug: aweber-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aweber/refs/heads/main/openapi/aweber-campaigns-api-openapi.yml
- filename: aweber-custom-fields-api-openapi.yml
  format: yaml
  label: AWeber Custom Fields API
  slug: aweber-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aweber/refs/heads/main/openapi/aweber-custom-fields-api-openapi.yml
- filename: aweber-landing-pages-api-openapi.yml
  format: yaml
  label: AWeber Landing Pages API
  slug: aweber-landing-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aweber/refs/heads/main/openapi/aweber-landing-pages-api-openapi.yml
- filename: aweber-lists-api-openapi.yml
  format: yaml
  label: AWeber Lists API
  slug: aweber-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aweber/refs/heads/main/openapi/aweber-lists-api-openapi.yml
- filename: aweber-segments-api-openapi.yml
  format: yaml
  label: AWeber Segments API
  slug: aweber-segments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aweber/refs/heads/main/openapi/aweber-segments-api-openapi.yml
- filename: aweber-subscribers-api-openapi.yml
  format: yaml
  label: AWeber Subscribers API
  slug: aweber-subscribers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aweber/refs/heads/main/openapi/aweber-subscribers-api-openapi.yml
- filename: aweber-web-forms-api-openapi.yml
  format: yaml
  label: AWeber Web Forms API
  slug: aweber-web-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aweber/refs/heads/main/openapi/aweber-web-forms-api-openapi.yml
- filename: aweber-integrations-api-openapi.yml
  format: yaml
  label: AWeber Integrations API
  slug: aweber-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aweber/refs/heads/main/openapi/aweber-integrations-api-openapi.yml
- filename: aweber-authentication-api-openapi.yml
  format: yaml
  label: AWeber Authentication API
  slug: aweber-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aweber/refs/heads/main/openapi/aweber-authentication-api-openapi.yml
- filename: aweber-beta-api-openapi.yml
  format: yaml
  label: AWeber Beta API
  slug: aweber-beta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aweber/refs/heads/main/openapi/aweber-beta-api-openapi.yml
certifications:
- PCI Security certification
- Privacy Shield certification
- GDPR
description: ''
kind: trust-center
layout: security
name: Aweber Trust Center
name_suffix: Trust Center
overview: AWeber maintains a public trust center documenting PCI Security certification, Privacy Shield certification, and GDPR compliance.
provider_name: AWeber
provider_slug: aweber
slug: aweber-trust-center
source_filename: aweber-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nprobe: true\nsource: https://www.aweber.com/dpst.htm\nurl: https://www.aweber.com/dpst.htm\nname: Data Processing & Security Terms\nnote: >-\n  AWeber has no dedicated trust center (trust.aweber.com and /trust both miss). Its compliance\n  posture is published as prose on the GDPR Data Processing & Security Terms page, reachable from\n  the Legal index at https://www.aweber.com/legal.htm. Two certifications are named with an\n  audit cadence; there is no SOC 2 report, ISO 27001 certificate, HIPAA or FedRAMP claim, and no\n  downloadable evidence or subprocessor list behind an NDA portal.\ncertifications:\n  - name: PCI Security certification\n    evidence: '\"Maintaining Payment Card Industry (PCI) Security certification by completing an annual compliance review\"'\n    source: https://www.aweber.com/dpst.htm\n  - name: Privacy Shield certification\n    evidence: '\"Maintaining Privacy-Shield certification by completing an annual third-party\
  \ review\"'\n    source: https://www.aweber.com/dpst.htm\n  - name: GDPR\n    evidence: Data Processing and Security Terms published as the customer-facing DPA.\n    source: https://www.aweber.com/dpst.htm\nmemberships:\n  - {name: M3AAWG, evidence: '\"AWeber is a proud member of M3AAWG\"', source: 'https://www.aweber.com/dpst.htm'}\npractices:\n  - Encryption of data in transit and at rest in AWeber data centers.\n  - Continual automated and manual monitoring of confidentiality and integrity.\ndata_rights:\n  documented: true\n  rights: [right to be informed, access, rectification, erasure, restriction, portability, objection]\n  source: https://www.aweber.com/dpst.htm\nrelated_policies:\n  - {name: Legal index, url: 'https://www.aweber.com/legal.htm'}\n  - {name: Privacy Policy, url: 'https://www.aweber.com/privacy.htm'}\n  - {name: Anti-Spam Policy, url: 'https://www.aweber.com/antispam.htm'}\n  - {name: Service Agreement, url: 'https://www.aweber.com/service-agreement.htm'}\n  - {name:\
  \ Developer Terms of Service, url: 'https://labs.aweber.com/docs/tos'}\nabsent:\n  - {item: trust.aweber.com, status: 'no such host / no trust portal'}\n  - {item: 'https://www.aweber.com/security', http_status: 404, checked: '2026-08-13'}\n  - {item: SOC 2, status: not published}\n  - {item: ISO 27001, status: not published}\nevidence:\n  - {source: 'https://www.aweber.com/dpst.htm', http_status: 200, keywords: [pci, privacy shield, gdpr, m3aawg, encryption]}\n  - {source: 'https://www.aweber.com/legal.htm', http_status: 200, keywords: [privacy, anti-spam, data processing, service agreement]}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aweber/refs/heads/main/security/aweber-trust-center.yml
summary_line: PCI Security certification, Privacy Shield certification, GDPR
tags:
- Email Marketing
- Marketing Automation
- Email
- Newsletters
- Subscribers
- Campaigns
- Landing Pages
- Web Forms
- Segments
- Webhooks
- OAuth 2.0
- Small Business
trust_url: https://www.aweber.com/dpst.htm
---
