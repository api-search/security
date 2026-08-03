---
api_specs:
- filename: hyperice-storefront-openapi.yml
  format: yaml
  label: Hyperice Storefront JSON API
  slug: hyperice-storefront-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperice/refs/heads/main/openapi/hyperice-storefront-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: hyperice.com
  spf: true
hosts:
- cert_expires: Oct 27 20:01:02 2026 GMT
  host: hyperice.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hyperice Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hyperice, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Hyperice
provider_slug: hyperice
slug: hyperice-domain-security
source_filename: hyperice-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hyperice.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 27 20:01:02 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: hyperice.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hyperice/refs/heads/main/security/hyperice-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Commerce
- Retail
- Health and Wellness
- Consumer Hardware
- Sports and Fitness
- Agentic Commerce
- GraphQL
- MCP
- Shopify
---
