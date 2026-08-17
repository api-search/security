---
api_specs:
- filename: sumble-contact-lists-api-openapi.yml
  format: yaml
  label: Sumble contact-lists API
  slug: sumble-contact-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sumble/refs/heads/main/openapi/sumble-contact-lists-api-openapi.yml
- filename: sumble-jobs-api-openapi.yml
  format: yaml
  label: Sumble jobs API
  slug: sumble-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sumble/refs/heads/main/openapi/sumble-jobs-api-openapi.yml
- filename: sumble-organization-lists-api-openapi.yml
  format: yaml
  label: Sumble organization-lists API
  slug: sumble-organization-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sumble/refs/heads/main/openapi/sumble-organization-lists-api-openapi.yml
- filename: sumble-organizations-api-openapi.yml
  format: yaml
  label: Sumble organizations API
  slug: sumble-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sumble/refs/heads/main/openapi/sumble-organizations-api-openapi.yml
- filename: sumble-people-api-openapi.yml
  format: yaml
  label: Sumble people API
  slug: sumble-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sumble/refs/heads/main/openapi/sumble-people-api-openapi.yml
- filename: sumble-projects-api-openapi.yml
  format: yaml
  label: Sumble projects API
  slug: sumble-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sumble/refs/heads/main/openapi/sumble-projects-api-openapi.yml
- filename: sumble-signals-api-openapi.yml
  format: yaml
  label: Sumble signals API
  slug: sumble-signals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sumble/refs/heads/main/openapi/sumble-signals-api-openapi.yml
- filename: sumble-support-api-openapi.yml
  format: yaml
  label: Sumble support API
  slug: sumble-support-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sumble/refs/heads/main/openapi/sumble-support-api-openapi.yml
- filename: sumble-teams-api-openapi.yml
  format: yaml
  label: Sumble teams API
  slug: sumble-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sumble/refs/heads/main/openapi/sumble-teams-api-openapi.yml
- filename: sumble-technologies-api-openapi.yml
  format: yaml
  label: Sumble technologies API
  slug: sumble-technologies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sumble/refs/heads/main/openapi/sumble-technologies-api-openapi.yml
certifications:
- SOC 2
- GDPR
description: ''
kind: trust-center
layout: security
name: Sumble Trust Center
name_suffix: Trust Center
overview: Sumble maintains a public trust center documenting SOC 2 and GDPR compliance.
provider_name: Sumble
provider_slug: sumble
slug: sumble-trust-center
source_filename: sumble-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nprobe: true\nurl: https://trust.sumble.com/\nplatform: Vanta Trust Center\nhttp_status: 200\nrendering: >-\n  JS-rendered Vanta shell — the certification list and report requests are\n  loaded client-side, so the certifications below are taken from Sumble's own\n  documentation rather than scraped from the trust center HTML.\ndocs: https://docs.sumble.com/trust-and-security/trust-and-security\ncertifications:\n  - SOC 2\n  - GDPR\nprograms:\n  - name: SOC 2\n    detail: Sumble maintains SOC 2 compliance; reports are requestable through the trust center.\n  - name: GDPR\n    detail: >-\n      Processes data in accordance with GDPR; people data sourced from public\n      professional profiles is handled per applicable data protection\n      regulations.\ninfrastructure:\n  provider: Google Cloud Platform (GCP)\n  encryption_in_transit: TLS for client traffic and internal service-to-service traffic\n  encryption_at_rest: GCP default encryption\
  \ at rest for all databases and storage\n  network_isolation: Production databases are not reachable from the public internet; access restricted to authorized services in the GCP project\n  access_controls: Least-privilege internal access; administrative actions logged to an audit trail\ndata_handling:\n  customer_isolation: Each customer's CRM data (accounts, contacts, enrichments) is logically isolated to authorized users in that customer's org\n  retention: Retained for the duration of the customer relationship; deletion on request\n  resale: 'CRM data shared for enrichment is used only to provide enrichment back to that customer — not shared with other customers and not sold'\nresponsible_ai:\n  own_models: Entity extraction, relationship classification and job-function classification over job-market data; no personal communications, private documents or sensitive personal information processed\n  llm_subprocessors:\n    - {vendor: Google, models: Gemini, use: 'user-facing intelligence\
  \ briefs (web app, REST API, MCP)'}\n    - {vendor: OpenAI, models: GPT, use: 'entity disambiguation, signal title generation'}\n    - {vendor: Anthropic, models: Claude, use: 'entity disambiguation, signal title generation'}\n  controls: Only structured business data and the prompt context required for the task are sent; LLM outputs are validated against structured data\nexternal_resources:\n  - {name: Trust center, url: 'https://trust.sumble.com/', status: 200}\n  - {name: System status, url: 'https://status.sumble.com/', status: 200}\nevidence:\n  - {source: 'https://trust.sumble.com/', status: 200, keywords: [vanta, trust center]}\n  - {source: 'https://docs.sumble.com/trust-and-security/trust-and-security.md', status: 200, keywords: [soc 2, gdpr, encryption, access controls, trust center]}\nchecked: '2026-08-13'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sumble/refs/heads/main/security/sumble-trust-center.yml
summary_line: SOC 2, GDPR
tags:
- Company
- Account Intelligence
- Sales Intelligence
- Data Enrichment
- Go-To-Market
- Technographics
- People Data
- Job Posts
- Signals
- MCP
trust_url: https://trust.sumble.com/
---
