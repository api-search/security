---
api_specs:
- filename: flagsmith-flags-api-openapi.yml
  format: yaml
  label: Flagsmith Flags API
  slug: flags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flagsmith/refs/heads/main/openapi/flagsmith-flags-api-openapi.yml
- filename: flagsmith-environments-api-openapi.yml
  format: yaml
  label: flagsmith Environments API
  slug: flagsmith-environments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flagsmith/refs/heads/main/openapi/flagsmith-environments-api-openapi.yml
- filename: flagsmith-features-api-openapi.yml
  format: yaml
  label: flagsmith Features API
  slug: flagsmith-features-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flagsmith/refs/heads/main/openapi/flagsmith-features-api-openapi.yml
- filename: flagsmith-identities-api-openapi.yml
  format: yaml
  label: flagsmith Identities API
  slug: flagsmith-identities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flagsmith/refs/heads/main/openapi/flagsmith-identities-api-openapi.yml
- filename: flagsmith-organisations-api-openapi.yml
  format: yaml
  label: flagsmith Organisations API
  slug: flagsmith-organisations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flagsmith/refs/heads/main/openapi/flagsmith-organisations-api-openapi.yml
- filename: flagsmith-projects-api-openapi.yml
  format: yaml
  label: flagsmith Projects API
  slug: flagsmith-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flagsmith/refs/heads/main/openapi/flagsmith-projects-api-openapi.yml
- filename: flagsmith-segments-api-openapi.yml
  format: yaml
  label: flagsmith Segments API
  slug: flagsmith-segments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flagsmith/refs/heads/main/openapi/flagsmith-segments-api-openapi.yml
- filename: flagsmith-users-api-openapi.yml
  format: yaml
  label: flagsmith Users API
  slug: flagsmith-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flagsmith/refs/heads/main/openapi/flagsmith-users-api-openapi.yml
- filename: flagsmith-webhooks-api-openapi.yml
  format: yaml
  label: flagsmith Webhooks API
  slug: flagsmith-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flagsmith/refs/heads/main/openapi/flagsmith-webhooks-api-openapi.yml
certification_count: 3
certifications:
- read
- note
- how_to_verify
description: 'Flagsmith runs a real, dedicated trust center on its own subdomain, built on Vanta. It is discoverable only if you already know the hostname: nothing on flagsmith.com under /security, /trust or /compliance resolves, and there is no security.txt on any host to point at it. That discoverability gap is the finding here — the programme exists and the front door is unsigned.'
kind: trust-center
layout: security
name: Flagsmith Trust Center
name_suffix: Trust Center
overview: Flagsmith maintains a public trust center documenting read, note, and how_to_verify compliance.
provider_name: Flagsmith
provider_slug: flagsmith
slug: flagsmith-trust-center
source_filename: flagsmith-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: probed\nsource: https://trust.flagsmith.com\nurl: https://trust.flagsmith.com\nplatform: Vanta\nhttp_status: 200\nchecked: '2026-09-17'\nevidence:\n- {url: 'https://trust.flagsmith.com', status: 200, content_type: 'text/html', observed: 'title \"Flagsmith Trust Center\"; Vanta-hosted (assets.vanta.com, app.vanta.com document links)'}\n- {url: 'https://flagsmith.com/security', status: 404}\n- {url: 'https://flagsmith.com/trust', status: 404}\n- {url: 'https://www.flagsmith.com/compliance', status: 404}\n- {url: 'https://flagsmith.com/.well-known/security.txt', status: 404}\ndescription: >-\n  Flagsmith runs a real, dedicated trust center on its own subdomain, built on Vanta. It is\n  discoverable only if you already know the hostname: nothing on flagsmith.com under /security,\n  /trust or /compliance resolves, and there is no security.txt on any host to point at it. That\n  discoverability gap is the finding here — the programme exists and the\
  \ front door is unsigned.\ncertifications:\n  read: false\n  note: >-\n    NOT RECORDED. The certification list and evidence documents are rendered client-side by the Vanta\n    application and gated behind a document request (app.vanta.com/doc?s=…), so no certification name\n    was readable anonymously. Nothing is asserted here — no SOC 2, ISO 27001, HIPAA, PCI or FedRAMP\n    claim is being made on Flagsmith's behalf from a page this probe could not read. Flagsmith's\n    pricing page markets \"Features for Maximum Security\" and its llms.txt names banking, financial\n    services and healthcare customers, but marketing copy is not a certification and is deliberately\n    not promoted to one.\n  how_to_verify: Open https://trust.flagsmith.com in a browser, or request documents through the Vanta portal.\ndocuments_gated: true\nsubprocessors: null\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flagsmith/refs/heads/main/security/flagsmith-trust-center.yml
summary_line: read, note, how_to_verify
tags:
- Feature Flags
- Remote Config
- Release Management
- A/B Testing
- Experimentation
- Segmentation
- Developer Tools
- DevOps
- Open-Source
- Software-as-a-Service
- MCP
- Agent Ready
trust_url: https://trust.flagsmith.com
---
