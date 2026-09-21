---
api_specs:
- filename: merchant-0-com-openapi.json
  format: json
  label: Merchant-0 A2A Protocol Server API
  slug: merchant-0-a2a-protocol-server-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/merchant-0-com/refs/heads/main/openapi/merchant-0-com-openapi.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: merchant-0.com
  spf: false
hosts:
- cert_expires: Nov  7 04:36:25 2026 GMT
  host: merchant-0.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  7 04:36:25 2026 GMT
  host: api.merchant-0.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Merchant 0 Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Merchant-0, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Merchant-0
provider_slug: merchant-0-com
slug: merchant-0-com-domain-security
source_filename: merchant-0-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: merchant-0.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  7 04:36:25 2026 GMT\n  hsts: false\n- host: api.merchant-0.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  7 04:36:25 2026 GMT\n  hsts: null\ndomains:\n- domain: merchant-0.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/merchant-0-com/refs/heads/main/security/merchant-0-com-domain-security.yml
summary_line: TLSv1.3
tags:
- Agents
- Agentic Commerce
- A2A
- AP2
- Universal Commerce Protocol
- Trade Intelligence
- Market Intelligence
- Supply Chain
- Southeast Asia
- Decentralized Identity
- agent-native
---
