---
api_specs:
- filename: monsitools-api-tools-json-api-openapi.yml
  format: yaml
  label: MonsiTools Api Tools.json API
  slug: monsitools-api-tools-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monsitools/refs/heads/main/openapi/monsitools-api-tools-json-api-openapi.yml
- filename: monsitools-calculate-api-openapi.yml
  format: yaml
  label: MonsiTools Calculate API
  slug: monsitools-calculate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monsitools/refs/heads/main/openapi/monsitools-calculate-api-openapi.yml
- filename: monsitools-keys-api-openapi.yml
  format: yaml
  label: MonsiTools Keys API
  slug: monsitools-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monsitools/refs/heads/main/openapi/monsitools-keys-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: monsitools.com
  spf: true
hosts:
- cert_expires: Nov 24 11:28:02 2026 GMT
  host: monsitools.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Monsitools Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MonsiTools, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: MonsiTools
provider_slug: monsitools
slug: monsitools-domain-security
source_filename: monsitools-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: monsitools.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 11:28:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: monsitools.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/monsitools/refs/heads/main/security/monsitools-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Calculators
- Finance
- Workflows
- MCP
- Data Tools
---
