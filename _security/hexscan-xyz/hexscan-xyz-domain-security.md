---
api_specs:
- filename: hexscan-xyz-health-api-openapi.yml
  format: yaml
  label: HexScan Health API
  slug: hexscan-xyz-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hexscan-xyz/openapi/hexscan-xyz-health-api-openapi.yml
- filename: hexscan-xyz-honeypot-api-openapi.yml
  format: yaml
  label: HexScan Honeypot API
  slug: hexscan-xyz-honeypot-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hexscan-xyz/openapi/hexscan-xyz-honeypot-api-openapi.yml
- filename: hexscan-xyz-llms-txt-api-openapi.yml
  format: yaml
  label: HexScan Llms.txt API
  slug: hexscan-xyz-llms-txt-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hexscan-xyz/openapi/hexscan-xyz-llms-txt-api-openapi.yml
- filename: hexscan-xyz-scan-api-openapi.yml
  format: yaml
  label: HexScan Scan API
  slug: hexscan-xyz-scan-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hexscan-xyz/openapi/hexscan-xyz-scan-api-openapi.yml
- filename: hexscan-xyz-simulate-api-openapi.yml
  format: yaml
  label: HexScan Simulate API
  slug: hexscan-xyz-simulate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hexscan-xyz/openapi/hexscan-xyz-simulate-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: hexscan.xyz
  spf: false
hosts:
- cert_expires: Dec 18 02:43:51 2026 GMT
  host: hexscan.xyz
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: HexScan Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HexScan, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: HexScan
provider_slug: hexscan-xyz
slug: hexscan-xyz-domain-security
source_filename: hexscan-xyz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hexscan.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 02:43:51 2026 GMT\n  hsts: false\ndomains:\n- domain: hexscan.xyz\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/hexscan-xyz/security/hexscan-xyz-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- TokenSecurity
- Cryptocurrency
- Blockchain
- Risk Assessment
---
