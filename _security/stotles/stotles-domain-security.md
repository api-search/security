---
api_specs:
- filename: stotles-buyers-api-openapi.yml
  format: yaml
  label: Stotles Buyers API
  slug: stotles-buyers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stotles/refs/heads/main/openapi/stotles-buyers-api-openapi.yml
- filename: stotles-frameworks-api-openapi.yml
  format: yaml
  label: Stotles Frameworks API
  slug: stotles-frameworks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stotles/refs/heads/main/openapi/stotles-frameworks-api-openapi.yml
- filename: stotles-notices-api-openapi.yml
  format: yaml
  label: Stotles Notices API
  slug: stotles-notices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stotles/refs/heads/main/openapi/stotles-notices-api-openapi.yml
- filename: stotles-suppliers-api-openapi.yml
  format: yaml
  label: Stotles Suppliers API
  slug: stotles-suppliers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stotles/refs/heads/main/openapi/stotles-suppliers-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: stotles.com
  spf: true
hosts:
- cert_expires: Sep 30 23:59:59 2026 GMT
  host: www.stotles.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 26 23:59:59 2026 GMT
  host: api.stotles.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Stotles Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Stotles, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Stotles
provider_slug: stotles
slug: stotles-domain-security
source_filename: stotles-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.stotles.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.stotles.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: stotles.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\nfindings:\n- id: api-host-no-hsts\n  severity: medium\n  detail: >-\n    api.stotles.com — the production API host and the MCP endpoint host — returns NO\n    Strict-Transport-Security header, while www.stotles.com sets one with max-age=31536000. A client\n    that first reaches the API over plain HTTP is not pinned to HTTPS for subsequent requests. This\n    matters more than usual here because authentication is a long-lived static `x-api-key` header:\n    a single downgraded request leaks\
  \ the organization's key.\n  observed: '2026-08-14'\n- id: no-dnssec\n  severity: low\n  detail: stotles.com is not DNSSEC-signed.\n  observed: '2026-08-14'\n- id: no-caa\n  severity: low\n  detail: >-\n    No CAA records are published for stotles.com, so no certificate authority is constrained from\n    issuing for the domain.\n  observed: '2026-08-14'\n- id: dmarc-quarantine-not-reject\n  severity: low\n  detail: DMARC policy is p=quarantine rather than p=reject.\n  observed: '2026-08-14'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stotles/refs/heads/main/security/stotles-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Procurement
- Public Sector
- Government
- Tenders
- Sales Intelligence
- B2G
- Market Intelligence
- OpenAPI
- MCP
- Agent Native
- Contract Awards
- Framework Agreements
- CPV
- United Kingdom
- Ireland
- GovTech
---
