---
api_specs:
- filename: chartervsown-com-calculator-api-openapi.yml
  format: yaml
  label: Charter vs Own Calculator API
  slug: chartervsown-com-calculator-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chartervsown-com/openapi/chartervsown-com-calculator-api-openapi.yml
- filename: chartervsown-com-enquiry-api-openapi.yml
  format: yaml
  label: Charter vs Own Enquiry API
  slug: chartervsown-com-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chartervsown-com/openapi/chartervsown-com-enquiry-api-openapi.yml
- filename: chartervsown-com-mcp-api-openapi.yml
  format: yaml
  label: Charter vs Own MCP API
  slug: chartervsown-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chartervsown-com/openapi/chartervsown-com-mcp-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: chartervsown.com
  spf: true
hosts:
- cert_expires: Jan 10 11:14:39 2027 GMT
  host: chartervsown.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Chartervsown Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Charter vs Own, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Charter vs Own
provider_slug: chartervsown-com
slug: chartervsown-com-domain-security
source_filename: chartervsown-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: chartervsown.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 11:14:39 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: chartervsown.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/chartervsown-com/security/chartervsown-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Aviation
- Finance
- Calculator
- Private-Jet
- CostEstimator
---
