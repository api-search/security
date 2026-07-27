---
api_specs:
- filename: purplebricks-property-v1-openapi.yml
  format: yaml
  label: Purplebricks Property API
  slug: purplebricks-property-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/purplebricks/refs/heads/main/openapi/purplebricks-property-v1-openapi.yml
- filename: purplebricks-account-v1-openapi.yml
  format: yaml
  label: Purplebricks Account API
  slug: purplebricks-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/purplebricks/refs/heads/main/openapi/purplebricks-account-v1-openapi.yml
- filename: purplebricks-valuations-v1-openapi.yml
  format: yaml
  label: Purplebricks Valuations API
  slug: purplebricks-valuations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/purplebricks/refs/heads/main/openapi/purplebricks-valuations-v1-openapi.yml
- filename: purplebricks-viewings-v1-openapi.yml
  format: yaml
  label: Purplebricks Viewings API
  slug: purplebricks-viewings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/purplebricks/refs/heads/main/openapi/purplebricks-viewings-v1-openapi.yml
- filename: purplebricks-messaging-v1-openapi.yml
  format: yaml
  label: Purplebricks Messaging API
  slug: purplebricks-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/purplebricks/refs/heads/main/openapi/purplebricks-messaging-v1-openapi.yml
- filename: purplebricks-lettings-v1-openapi.yml
  format: yaml
  label: Purplebricks Lettings API
  slug: purplebricks-lettings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/purplebricks/refs/heads/main/openapi/purplebricks-lettings-v1-openapi.yml
- filename: purplebricks-branch-v1-openapi.yml
  format: yaml
  label: Purplebricks Branch API
  slug: purplebricks-branch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/purplebricks/refs/heads/main/openapi/purplebricks-branch-v1-openapi.yml
- filename: purplebricks-communications-v1-openapi.yml
  format: yaml
  label: Purplebricks Communications API
  slug: purplebricks-communications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/purplebricks/refs/heads/main/openapi/purplebricks-communications-v1-openapi.yml
- filename: purplebricks-conveyancing-v1-openapi.yml
  format: yaml
  label: Purplebricks Conveyancing API
  slug: purplebricks-conveyancing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/purplebricks/refs/heads/main/openapi/purplebricks-conveyancing-v1-openapi.yml
- filename: purplebricks-agent-v1-openapi.yml
  format: yaml
  label: Purplebricks Agent API
  slug: purplebricks-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/purplebricks/refs/heads/main/openapi/purplebricks-agent-v1-openapi.yml
- filename: purplebricks-feedback-v1-openapi.yml
  format: yaml
  label: Purplebricks Feedback API
  slug: purplebricks-feedback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/purplebricks/refs/heads/main/openapi/purplebricks-feedback-v1-openapi.yml
- filename: purplebricks-workflow-v1-openapi.yml
  format: yaml
  label: Purplebricks Workflow API
  slug: purplebricks-workflow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/purplebricks/refs/heads/main/openapi/purplebricks-workflow-v1-openapi.yml
- filename: purplebricks-outlook-v1-openapi.yml
  format: yaml
  label: Purplebricks Outlook Sync API
  slug: purplebricks-outlook-sync-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/purplebricks/refs/heads/main/openapi/purplebricks-outlook-v1-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: purplebricks.co.uk
  spf: true
hosts:
- cert_expires: Nov 12 23:59:59 2026 GMT
  host: www.purplebricks.co.uk
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 15 23:59:59 2026 GMT
  host: api.purplebricks.co.uk
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Purplebricks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Purplebricks, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Purplebricks
provider_slug: purplebricks
slug: purplebricks-domain-security
source_filename: purplebricks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.purplebricks.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.purplebricks.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: purplebricks.co.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/purplebricks/refs/heads/main/security/purplebricks-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Real Estate
- United Kingdom
- Property Listings
- Online Estate Agency
- Rentals
- Lettings
- PropTech
- Mortgage
- Conveyancing
- Land Registry
- OpenAPI
- Microservices
- Swagger
- Azure
---
