---
api_specs:
- filename: cogny-reports-api-openapi.yml
  format: yaml
  label: Cogny Reports API
  slug: cogny-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cogny/refs/heads/main/openapi/cogny-reports-api-openapi.yml
- filename: cogny-tickets-api-openapi.yml
  format: yaml
  label: Cogny Tickets API
  slug: cogny-tickets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cogny/refs/heads/main/openapi/cogny-tickets-api-openapi.yml
- filename: cogny-warehouses-api-openapi.yml
  format: yaml
  label: Cogny Warehouses API
  slug: cogny-warehouses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cogny/refs/heads/main/openapi/cogny-warehouses-api-openapi.yml
- filename: cogny-webhooks-api-openapi.yml
  format: yaml
  label: Cogny Webhooks API
  slug: cogny-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cogny/refs/heads/main/openapi/cogny-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cogny.com
  spf: true
hosts:
- cert_expires: Sep 27 15:42:53 2026 GMT
  host: cogny.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 30 03:52:33 2026 GMT
  host: api.cogny.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cogny Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cogny, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Cogny
provider_slug: cogny
slug: cogny-domain-security
source_filename: cogny-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cogny.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 15:42:53 2026 GMT\n  hsts: false\n- host: api.cogny.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 03:52:33 2026 GMT\n  hsts: null\ndomains:\n- domain: cogny.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cogny/refs/heads/main/security/cogny-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Ai Enterprise Software
- Marketing
- Marketing Analytics
- Marketing Automation
- MCP
- Agents
- Data Warehouse
- Advertising
---
