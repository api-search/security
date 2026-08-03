---
api_specs:
- filename: anecdotes-grc-openapi.yml
  format: yaml
  label: Anecdotes GRC API
  slug: anecdotes-grc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anecdotes/refs/heads/main/openapi/anecdotes-grc-openapi.yml
- filename: anecdotes-fedramp-20x-openapi.yml
  format: yaml
  label: Anecdotes FedRAMP 20x Trust Center API
  slug: anecdotes-fedramp-20x-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anecdotes/refs/heads/main/openapi/anecdotes-fedramp-20x-openapi.yml
certifications:
- SOC 1
- SOC 2
- ISO 27001
- ISO 27701
- ISO 27032
- ISO 42001
- GDPR
description: ''
kind: trust-center
layout: security
name: Anecdotes Trust Center
name_suffix: Trust Center
overview: anecdotes maintains a public trust center documenting SOC 1, SOC 2, ISO 27001, ISO 27701, ISO 27032, ISO 42001, and GDPR compliance.
provider_name: anecdotes
provider_slug: anecdotes
slug: anecdotes-trust-center
source_filename: anecdotes-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-07-31'\nmethod: searched\nprobe: true\nsource: https://www.anecdotes.ai/trust\nurl: https://trust.anecdotes.ai/\nsecurity_page: https://www.anecdotes.ai/trust\nsummary: >-\n  Anecdotes runs its trust center on its own product - trust.anecdotes.ai is an instance of the Anecdotes\n  Trust Center, which is itself one of the two Cloud Service Offerings in its FedRAMP 20x package. Gated\n  documents are released behind a request-access and NDA flow. Uniquely among providers in this catalog,\n  the trust center is also queryable as an API: the FedRAMP 20x public endpoints return CSO metadata,\n  status-page uptime and the Recommended Secure Configuration index with no authentication at all.\ncertifications:\n- SOC 1\n- SOC 2\n- ISO 27001\n- ISO 27701\n- ISO 27032\n- ISO 42001\n- GDPR\nprograms:\n- name: FedRAMP 20x\n  impact_level: Moderate\n  deployment_model: Public Cloud\n  service_model: SaaS\n  cloud_service_offerings:\n  - Anecdotes Compliance OS\n  - Anecdotes\
  \ Trust Center\n  docs: https://help.anecdotes.ai/technical-setup/fedramp-20x-trust-center-and-api\npractices:\n  penetration_testing: External vendors, at least once every 12 months.\n  encryption_at_rest: AES-256\n  encryption_in_transit: TLS 1.2 and above\n  hosting: Google Cloud Platform, US data centers\n  dpa: offered for GDPR compliance\n  subprocessors: published\naccess_model:\n  public: CSO metadata, status page rollup, Recommended Secure Configuration index, API documentation and Postman collection\n  gated: authorization package, Key Security Indicators, evidence and evidence history\n  gating: request access (name, email, company, job title) then approval and NDA\nmachine_readable:\n  api: https://help.anecdotes.ai/technical-setup/fedramp-20x-trust-center-and-api\n  openapi: openapi/anecdotes-fedramp-20x-openapi.yml\n  postman: postman/anecdotes-fedramp-20x.postman_collection.json\n  public_endpoint_verified:\n    url: https://api.anecdotes.ai/fedramp20x/v1/public/info?evidence_id=url_2037408219127\n\
  \    http_status: 200\n    fetched: '2026-07-31'\ncontacts:\n  security: security@anecdotes.ai\n  support: support@anecdotes.ai\n  general: hello@anecdotes.ai\nevidence:\n- source: https://www.anecdotes.ai/trust\n  keywords: [soc 1, soc 2, iso 27001, iso 27701, iso 27032, iso 42001, gdpr, penetration test, trust center]\n- source: https://trust.anecdotes.ai/\n  http_status: 200\n  note: Client-rendered trust center application; certification detail is rendered client-side.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anecdotes/refs/heads/main/security/anecdotes-trust-center.yml
summary_line: SOC 1, SOC 2, ISO 27001, ISO 27701, ISO 27032, ISO 42001, GDPR
tags:
- Company
- Compliance
- Governance
- Risk
- Security
- GRC
- Audit
- Evidence
- Continuous Compliance
- FedRAMP
- Artificial Intelligence
- Agents
trust_url: https://trust.anecdotes.ai/
---
