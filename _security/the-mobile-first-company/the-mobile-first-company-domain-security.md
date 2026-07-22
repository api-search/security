---
api_specs:
- filename: the-mobile-first-company-allo-openapi.json
  format: json
  label: Allo API
  slug: allo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-mobile-first-company/refs/heads/main/openapi/the-mobile-first-company-allo-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: withallo.com
  spf: true
hosts:
- cert_expires: Sep 21 13:00:33 2026 GMT
  host: api.withallo.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: The Mobile First Company Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for The Mobile First Company, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: The Mobile First Company
provider_slug: the-mobile-first-company
slug: the-mobile-first-company-domain-security
source_filename: the-mobile-first-company-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.withallo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 13:00:33 2026 GMT\n  hsts: null\ndomains:\n- domain: withallo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/the-mobile-first-company/refs/heads/main/security/the-mobile-first-company-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Communication
- Telephony
- Voice
- SMS
- CRM
- Artificial Intelligence
- MCP
- Webhooks
- Small Business
---
