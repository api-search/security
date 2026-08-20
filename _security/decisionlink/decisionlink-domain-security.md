---
api_specs:
- filename: decisionlink-value-proposition-openapi.yml
  format: yaml
  label: Xfactor.io Value Proposition API
  slug: xfactorio-value-proposition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/decisionlink/refs/heads/main/openapi/decisionlink-value-proposition-openapi.yml
- filename: decisionlink-value-facts-openapi.yml
  format: yaml
  label: Xfactor.io Value Facts API
  slug: xfactorio-value-facts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/decisionlink/refs/heads/main/openapi/decisionlink-value-facts-openapi.yml
- filename: decisionlink-value-chat-openapi.yml
  format: yaml
  label: Xfactor.io Value Chat API
  slug: xfactorio-value-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/decisionlink/refs/heads/main/openapi/decisionlink-value-chat-openapi.yml
- filename: decisionlink-collaboration-openapi.yml
  format: yaml
  label: Xfactor.io Collaboration Manager API
  slug: xfactorio-collaboration-manager-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/decisionlink/refs/heads/main/openapi/decisionlink-collaboration-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: xfactor.io
  spf: true
hosts:
- cert_expires: Nov  6 06:07:35 2026 GMT
  host: www.xfactor.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 28 23:59:59 2026 GMT
  host: api.xfactor.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Decisionlink Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DecisionLink, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: DecisionLink
provider_slug: decisionlink
slug: decisionlink-domain-security
source_filename: decisionlink-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.xfactor.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 06:07:35 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.xfactor.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: xfactor.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/decisionlink/refs/heads/main/security/decisionlink-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Cloud Saas
- Revenue Operations
- Customer Value Management
- Artificial Intelligence
- Go-To-Market
- Sales
- Analytics
- Value Selling
- Forecasting
---
