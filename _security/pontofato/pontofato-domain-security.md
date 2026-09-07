---
api_specs:
- filename: openapi.json
  format: json
  label: PontoFato API
  slug: pontofato-api
  spec_type: OpenAPI
  url: https://pontofato.com/openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: pontofato.com
  spf: true
hosts:
- cert_expires: Nov 29 14:41:36 2026 GMT
  host: pontofato.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Pontofato Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PontoFato, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: PontoFato
provider_slug: pontofato
slug: pontofato-domain-security
source_filename: pontofato-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pontofato.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 29 14:41:36 2026 GMT\n  hsts: false\ndomains:\n- domain: pontofato.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pontofato/refs/heads/main/security/pontofato-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Brazilian CEP
- address geocoding
- IBGE CNEFE
- geospatial
- latitude/longitude
- CNPJ
- Receita Federal
- business registry
- location intelligence
- proximity search
- radius search
- open government data
- agent-native
- MCP
- x402 micropayments
---
