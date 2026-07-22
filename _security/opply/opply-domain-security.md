---
api_specs:
- filename: opply-openapi-original.yml
  format: yaml
  label: Opply API
  slug: opply-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opply/refs/heads/main/openapi/opply-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: opply.com
  spf: true
hosts:
- cert_expires: Oct  3 16:09:58 2026 GMT
  host: opply.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 16:09:58 2026 GMT
  host: api.opply.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Opply Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Opply, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Opply
provider_slug: opply
slug: opply-domain-security
source_filename: opply-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: opply.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 16:09:58 2026 GMT\n  hsts: false\n- host: api.opply.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 16:09:58 2026 GMT\n  hsts: null\ndomains:\n- domain: opply.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opply/refs/heads/main/security/opply-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Food and Beverage
- Supply Chain
- Procurement
- Ordering
- Payments
- Sourcing
- Logistics
- AI Agents
- MCP
---
