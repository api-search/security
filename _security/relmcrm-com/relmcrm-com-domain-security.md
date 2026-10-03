---
api_specs:
- filename: relmcrm-com-activities-api-openapi.yml
  format: yaml
  label: Relm Activities API
  slug: relmcrm-com-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/relmcrm-com/refs/heads/main/openapi/relmcrm-com-activities-api-openapi.yml
- filename: relmcrm-com-automations-api-openapi.yml
  format: yaml
  label: Relm Automations API
  slug: relmcrm-com-automations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/relmcrm-com/refs/heads/main/openapi/relmcrm-com-automations-api-openapi.yml
- filename: relmcrm-com-batch-api-openapi.yml
  format: yaml
  label: Relm Batch API
  slug: relmcrm-com-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/relmcrm-com/refs/heads/main/openapi/relmcrm-com-batch-api-openapi.yml
- filename: relmcrm-com-companies-api-openapi.yml
  format: yaml
  label: Relm Companies API
  slug: relmcrm-com-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/relmcrm-com/refs/heads/main/openapi/relmcrm-com-companies-api-openapi.yml
- filename: relmcrm-com-connections-api-openapi.yml
  format: yaml
  label: Relm Connections API
  slug: relmcrm-com-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/relmcrm-com/refs/heads/main/openapi/relmcrm-com-connections-api-openapi.yml
- filename: relmcrm-com-contacts-api-openapi.yml
  format: yaml
  label: Relm Contacts API
  slug: relmcrm-com-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/relmcrm-com/refs/heads/main/openapi/relmcrm-com-contacts-api-openapi.yml
- filename: relmcrm-com-deals-api-openapi.yml
  format: yaml
  label: Relm Deals API
  slug: relmcrm-com-deals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/relmcrm-com/refs/heads/main/openapi/relmcrm-com-deals-api-openapi.yml
- filename: relmcrm-com-discovery-api-openapi.yml
  format: yaml
  label: Relm Discovery API
  slug: relmcrm-com-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/relmcrm-com/refs/heads/main/openapi/relmcrm-com-discovery-api-openapi.yml
- filename: relmcrm-com-pipelines-api-openapi.yml
  format: yaml
  label: Relm Pipelines API
  slug: relmcrm-com-pipelines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/relmcrm-com/refs/heads/main/openapi/relmcrm-com-pipelines-api-openapi.yml
- filename: relmcrm-com-registry-api-openapi.yml
  format: yaml
  label: Relm Registry API
  slug: relmcrm-com-registry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/relmcrm-com/refs/heads/main/openapi/relmcrm-com-registry-api-openapi.yml
- filename: relmcrm-com-search-api-openapi.yml
  format: yaml
  label: Relm Search API
  slug: relmcrm-com-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/relmcrm-com/refs/heads/main/openapi/relmcrm-com-search-api-openapi.yml
- filename: relmcrm-com-sequences-api-openapi.yml
  format: yaml
  label: Relm Sequences API
  slug: relmcrm-com-sequences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/relmcrm-com/refs/heads/main/openapi/relmcrm-com-sequences-api-openapi.yml
- filename: relmcrm-com-templates-api-openapi.yml
  format: yaml
  label: Relm Templates API
  slug: relmcrm-com-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/relmcrm-com/refs/heads/main/openapi/relmcrm-com-templates-api-openapi.yml
- filename: relmcrm-com-webhooks-api-openapi.yml
  format: yaml
  label: Relm Webhooks API
  slug: relmcrm-com-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/relmcrm-com/refs/heads/main/openapi/relmcrm-com-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: relmcrm.com
  spf: true
hosts:
- cert_expires: Nov 28 20:04:17 2026 GMT
  host: relmcrm.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 28 20:04:17 2026 GMT
  host: api.relmcrm.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Relmcrm Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Relm, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Relm
provider_slug: relmcrm-com
slug: relmcrm-com-domain-security
source_filename: relmcrm-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: relmcrm.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 20:04:17 2026 GMT\n  hsts: false\n- host: api.relmcrm.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 20:04:17 2026 GMT\n  hsts: false\ndomains:\n- domain: relmcrm.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/relmcrm-com/refs/heads/main/security/relmcrm-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- CRM
- Sales
- Contacts
- Deals
- Sales Pipeline
- Automation
- Webhook
- MCP
- A2A
- AI Agents
- Agent-Native
- United Arab Emirates
---
