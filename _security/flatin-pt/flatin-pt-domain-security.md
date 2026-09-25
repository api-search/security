---
api_specs:
- filename: flatin-pt-openapi.json
  format: json
  label: flatin.pt API
  slug: flatinpt-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flatin-pt/refs/heads/main/openapi/flatin-pt-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: flatin.pt
  spf: true
hosts:
- cert_expires: Dec  6 22:56:22 2026 GMT
  host: flatin.pt
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Flatin Pt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for flatin.pt, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: flatin.pt
provider_slug: flatin-pt
slug: flatin-pt-domain-security
source_filename: flatin-pt-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: flatin.pt\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  6 22:56:22 2026 GMT\n  hsts: false\ndomains:\n- domain: flatin.pt\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flatin-pt/refs/heads/main/security/flatin-pt-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Real Estate
- Property Tax
- Tax
- IMI
- IMT
- Stamp Duty
- Portugal
- Open Data
- Government Data
- Fiscal Data
- MCP
- AI Agents
---
