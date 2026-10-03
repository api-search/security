---
api_specs:
- filename: movehome-org-branches-api-openapi.yml
  format: yaml
  label: Move Home Organisation CIC Branches API
  slug: movehome-org-branches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/movehome-org/refs/heads/main/openapi/movehome-org-branches-api-openapi.yml
- filename: movehome-org-listings-api-openapi.yml
  format: yaml
  label: Move Home Organisation CIC Listings API
  slug: movehome-org-listings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/movehome-org/refs/heads/main/openapi/movehome-org-listings-api-openapi.yml
- filename: movehome-org-operational-api-openapi.yml
  format: yaml
  label: Move Home Organisation CIC Operational API
  slug: movehome-org-operational-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/movehome-org/refs/heads/main/openapi/movehome-org-operational-api-openapi.yml
- filename: movehome-org-products-api-openapi.yml
  format: yaml
  label: Move Home Organisation CIC Products API
  slug: movehome-org-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/movehome-org/refs/heads/main/openapi/movehome-org-products-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: movehome.org
  spf: false
hosts:
- cert_expires: Nov  1 07:29:18 2026 GMT
  host: movehome.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Movehome Org Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Move Home Organisation CIC, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Move Home Organisation CIC
provider_slug: movehome-org
slug: movehome-org-domain-security
source_filename: movehome-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: movehome.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 07:29:18 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: movehome.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/movehome-org/refs/heads/main/security/movehome-org-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Real Estate
- Property
- Lettings
- Property Sales
- Agents
- A2A
- MCP
- Agent-Native
- Agent Registry
- Non-Profit
- Open Source
- RAIA Protocol
- United Kingdom
---
