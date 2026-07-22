---
api_specs:
- filename: voidpet-discovery-openapi.json
  format: json
  label: Voidpet Public Discovery API
  slug: voidpet-public-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/voidpet/refs/heads/main/openapi/voidpet-discovery-openapi.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: voidpet.com
  spf: true
hosts:
- cert_expires: Aug 22 20:59:10 2026 GMT
  host: voidpet.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Voidpet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Voidpet, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Voidpet
provider_slug: voidpet
slug: voidpet-domain-security
source_filename: voidpet-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: voidpet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 20:59:10 2026 GMT\n  hsts: false\ndomains:\n- domain: voidpet.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/voidpet/refs/heads/main/security/voidpet-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Company
- Games
- Gaming
- Mental Health
- Wellness
- Discovery
- Agents
- MCP
- Read Only
---
