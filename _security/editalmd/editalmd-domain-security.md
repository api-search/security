---
api_specs:
- filename: openapi.json
  format: json
  label: EditalMD API
  slug: editalmd-api
  spec_type: OpenAPI
  url: https://editalmd.com/openapi.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: editalmd.com
  spf: true
hosts:
- cert_expires: Nov 29 20:55:51 2026 GMT
  host: editalmd.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Editalmd Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EditalMD, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: EditalMD
provider_slug: editalmd
slug: editalmd-domain-security
source_filename: editalmd-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: editalmd.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 29 20:55:51 2026 GMT\n  hsts: false\ndomains:\n- domain: editalmd.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/editalmd/refs/heads/main/security/editalmd-domain-security.yml
summary_line: TLSv1.3
tags:
- GovTech
- Public Procurement
- Brazil
- PNCP
- Legal & Compliance
- Business Intelligence
- Company Data
- CNPJ
- CNAE
- SICAF
- Document Extraction
- Agent-Native
- MCP
- x402
- Machine-Payable
---
