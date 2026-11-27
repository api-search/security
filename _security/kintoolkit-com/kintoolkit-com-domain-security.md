---
api_specs:
- filename: kintoolkit-com-discovery-api-openapi.yml
  format: yaml
  label: KinToolkit Discovery API
  slug: kintoolkit-com-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kintoolkit-com/openapi/kintoolkit-com-discovery-api-openapi.yml
- filename: kintoolkit-com-mcp-api-openapi.yml
  format: yaml
  label: KinToolkit MCP API
  slug: kintoolkit-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kintoolkit-com/openapi/kintoolkit-com-mcp-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: kintoolkit.com
  spf: false
hosts:
- cert_expires: Dec 16 01:53:25 2026 GMT
  host: kintoolkit.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: KinToolkit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for KinToolkit, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: KinToolkit
provider_slug: kintoolkit-com
slug: kintoolkit-com-domain-security
source_filename: kintoolkit-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kintoolkit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 01:53:25 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: kintoolkit.com\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/kintoolkit-com/security/kintoolkit-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Healthcare
- Dosage Calculator
- Pediatrics
- Medication
---
