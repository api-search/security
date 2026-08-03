---
api_specs:
- filename: datarails-financeos-mcp-openapi.json
  format: json
  label: Datarails FinanceOS MCP Server
  slug: financeos-mcp
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datarails/refs/heads/main/openapi/datarails-financeos-mcp-openapi.json
certifications:
- SOC 2 Type II
- ISO 27001
- GDPR
description: Datarails operates a hosted trust center at trust.datarails.com, reached from the marketing site via /compliance-and-legal-documents/ (HTTP 301). The trust center itself is a Nuxt single-page application whose certification list is loaded client-side from the Vendict API, so the certifications below are NOT scraped from it — they are taken verbatim from Datarails' own support documentation, which is a first-party published claim with a citable URL.
kind: trust-center
layout: security
name: Datarails Trust Center
name_suffix: Trust Center
overview: Datarails maintains a public trust center documenting SOC 2 Type II, ISO 27001, and GDPR compliance.
provider_name: Datarails
provider_slug: datarails
slug: datarails-trust-center
source_filename: datarails-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: searched\nprobe: true\nurl: https://trust.datarails.com/\ncanonical_entry: https://www.datarails.com/compliance-and-legal-documents/\nplatform: Vendict\ndescription: >-\n  Datarails operates a hosted trust center at trust.datarails.com, reached from\n  the marketing site via /compliance-and-legal-documents/ (HTTP 301). The trust\n  center itself is a Nuxt single-page application whose certification list is\n  loaded client-side from the Vendict API, so the certifications below are NOT\n  scraped from it — they are taken verbatim from Datarails' own support\n  documentation, which is a first-party published claim with a citable URL.\n\ncertifications:\n  - name: SOC 2 Type II\n    source: https://support.datarails.com/hc/en-us/articles/25873904696860-Getting-Started-with-Datarails-on-Claude-Desktop\n    claim: 'Datarails is SOC 2 Type II, GDPR, and ISO 27001 certified.'\n    evidence_type: provider documentation\n  - name: ISO 27001\n    source:\
  \ https://support.datarails.com/hc/en-us/articles/25873904696860-Getting-Started-with-Datarails-on-Claude-Desktop\n    claim: 'Datarails is SOC 2 Type II, GDPR, and ISO 27001 certified.'\n    evidence_type: provider documentation\n  - name: GDPR\n    source: https://support.datarails.com/hc/en-us/articles/25873904696860-Getting-Started-with-Datarails-on-Claude-Desktop\n    claim: 'Datarails is SOC 2 Type II, GDPR, and ISO 27001 certified.'\n    evidence_type: provider documentation\n    note: A regulation, not a certification; recorded as Datarails states it.\n\ndocuments:\n  - name: Security and compliance documentation\n    url: https://www.datarails.com/datarails-security-and-compliance-documents/\n    redirects_to: https://trust.datarails.com/overview/\n    note: >-\n      The support article \"Datarails Security and Compliance\" points here; the\n      page 301-redirects into the trust center, where document access is gated.\n  - name: Privacy Policy\n    url: https://www.datarails.com/privacy-policy/\n\
  \    last_updated: '2026-03-23'\n    contact: compliance@datarails.com\n  - name: Terms of Service\n    url: https://www.datarails.com/terms-of-service/\n    last_updated: '2026-03-15'\n  - name: AI Terms\n    url: https://www.datarails.com/datarails-ai-terms/\n    last_updated: '2026-03-15'\n    note: Separate published terms governing Datarails' use of AI.\n\ngated_document_set:\n  note: >-\n    The retired /datarails-security-and-compliance-documents/ page rendered one\n    tile per downloadable document, and the tile image slugs survive in the\n    WordPress page sitemap. They enumerate the document set Datarails makes\n    available behind the trust center. The DOCUMENTS THEMSELVES ARE GATED and\n    were not retrieved; only their names are recorded.\n  source: https://www.datarails.com/page-sitemap.xml\n  documents:\n    - SOC 1 Type II\n    - Security white paper\n    - Technical and architecture overview\n    - Penetration test statement\n    - Incident response plan\n    - HIPAA\
  \ compliance\n    - GDPR terms\n    - Terms and conditions\n  caveat: >-\n    A tile named \"soc-1-type-ii\" is evidence of a SOC 1 Type II report, which is\n    a different attestation from the SOC 2 Type II Datarails claims in its\n    support documentation. Both are recorded; neither report was seen.\n\nrelated_pages:\n  - https://support.datarails.com/hc/en-us/articles/6160603869073-Datarails-Security-and-Compliance\n  - https://support.datarails.com/hc/en-us/articles/5568068213265-Data-Privacy\n\nai_data_handling:\n  source: https://support.datarails.com/hc/en-us/articles/25849710214556-Datarails-FinanceOS-MCP-Server-Technical-Documentation\n  hosting_region: United States\n  transport_encryption: HTTPS in transit\n  minimisation: Only the data required to fulfil a specific request is transmitted.\n  replication: No full dataset replication occurs as part of the MCP integration.\n  access_boundary: Access remains limited to the caller's existing Datarails user permissions.\n  read_only:\
  \ The MCP connection cannot create, update or delete records.\n\nx-evidence:\n  fetched: '2026-08-01'\n  probes:\n    - {url: 'https://trust.datarails.com/', http_status: 200, note: 'Nuxt SPA shell; certification list not present in the served HTML'}\n    - {url: 'https://www.datarails.com/datarails-security-and-compliance-documents/', http_status: 301, location: 'https://trust.datarails.com/overview/'}\n    - {url: 'https://trust.datarails.com/overview/', http_status: 404, note: 'Direct fetch of the deep link 404s; the SPA routes it client-side'}\n  keywords_confirmed: [trust center, compliance, security]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/datarails/refs/heads/main/security/datarails-trust-center.yml
summary_line: SOC 2 Type II, ISO 27001, GDPR
tags:
- Company
- FP&A
- Financial Planning
- Finance
- Accounting
- Budgeting
- Forecasting
- Business Intelligence
- Reporting
- Data Integration
- Model Context Protocol
- Artificial Intelligence
- Excel
- SaaS
trust_url: https://trust.datarails.com/
---
