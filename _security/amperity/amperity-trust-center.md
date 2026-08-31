---
api_specs:
- filename: amperity-audit-events-api-openapi.yml
  format: yaml
  label: Amperity Audit Events API
  slug: amperity-audit-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amperity/refs/heads/main/openapi/amperity-audit-events-api-openapi.yml
- filename: amperity-campaigns-api-openapi.yml
  format: yaml
  label: Amperity Campaigns API
  slug: amperity-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amperity/refs/heads/main/openapi/amperity-campaigns-api-openapi.yml
- filename: amperity-ingest-api-openapi.yml
  format: yaml
  label: Amperity Ingest API
  slug: amperity-ingest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amperity/refs/heads/main/openapi/amperity-ingest-api-openapi.yml
- filename: amperity-segments-api-openapi.yml
  format: yaml
  label: Amperity Segments API
  slug: amperity-segments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amperity/refs/heads/main/openapi/amperity-segments-api-openapi.yml
- filename: amperity-workflow-api-openapi.yml
  format: yaml
  label: Amperity Workflow API
  slug: amperity-workflow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amperity/refs/heads/main/openapi/amperity-workflow-api-openapi.yml
certifications: []
description: 'Amperity''s published trust surface. Its own meta description states: "Amperity helps organizations turn complex customer data into trusted intelligence. Protecting that data is fundamental to everything we build. Our Trust Center provides transparent access to information about our security, privacy, compliance, and governance practices so you can confidently understand how Amperity safeguards your data."'
kind: trust-center
layout: security
name: Amperity Trust Center
name_suffix: Trust Center
overview: Amperity maintains a public trust center covering its security and compliance posture.
provider_name: Amperity
provider_slug: amperity
slug: amperity-trust-center
source_filename: amperity-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nprobe: true\nsource: https://trust.amperity.com/\nurl: https://trust.amperity.com/\nchecked: '2026-08-13'\nplatform: Vanta Trust Center\ntitle: Amperity Trust Center\ndescription: >-\n  Amperity's published trust surface. Its own meta description states: \"Amperity helps organizations\n  turn complex customer data into trusted intelligence. Protecting that data is fundamental to\n  everything we build. Our Trust Center provides transparent access to information about our security,\n  privacy, compliance, and governance practices so you can confidently understand how Amperity\n  safeguards your data.\"\ncovers: [security, privacy, compliance, governance]\ncertifications: []\ncertifications_note: >-\n  NOT recorded as \"none\". The Vanta trust center renders its control and certification list entirely\n  client-side from a JavaScript bundle - the server-delivered HTML is a 7 KB shell carrying only the\n  title and meta description, and\
  \ every /api/* path under both trust.amperity.com and app.vanta.com\n  answers 200 with that same shell. No named certification (SOC 2, ISO 27001, PCI DSS, HIPAA, FedRAMP)\n  could be read without executing JavaScript, so none is asserted here. A follow-up pass with a\n  headless browser would resolve it. Absence of evidence, recorded as such.\ndocument_access:\n  model: gated\n  note: >-\n    Vanta trust centers typically place audit reports behind an NDA/request flow. Whether Amperity's\n    documents are open or gated could not be established from the static shell.\nevidence:\n- source: https://trust.amperity.com/\n  http_status: 200\n  content_type: text/html\n  keywords: [trust center, security, compliance, privacy, governance]\n  fetched: '2026-08-13'\n- source: https://security.amperity.com/\n  http_status: 000\n  note: 'Does not resolve. Checked so the negative is on record.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amperity/refs/heads/main/security/amperity-trust-center.yml
summary_line: trust center published
tags:
- Company
- Enterprise
- Customer Data Platform
- CDP
- Identity Resolution
- Customer 360
- Marketing
- Data
- Profiles
- Analytics
- MCP
- Agents
- Retail
- Identity
trust_url: https://trust.amperity.com/
---
