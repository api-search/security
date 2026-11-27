---
api_specs:
- filename: costbench-com-compare-api-openapi.yml
  format: yaml
  label: CostBench Compare API
  slug: costbench-com-compare-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/costbench-com/openapi/costbench-com-compare-api-openapi.yml
- filename: costbench-com-coverage-api-openapi.yml
  format: yaml
  label: CostBench Coverage API
  slug: costbench-com-coverage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/costbench-com/openapi/costbench-com-coverage-api-openapi.yml
- filename: costbench-com-discover-api-openapi.yml
  format: yaml
  label: CostBench Discover API
  slug: costbench-com-discover-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/costbench-com/openapi/costbench-com-discover-api-openapi.yml
- filename: costbench-com-history-api-openapi.yml
  format: yaml
  label: CostBench History API
  slug: costbench-com-history-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/costbench-com/openapi/costbench-com-history-api-openapi.yml
- filename: costbench-com-mcp-api-openapi.yml
  format: yaml
  label: CostBench MCP API
  slug: costbench-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/costbench-com/openapi/costbench-com-mcp-api-openapi.yml
- filename: costbench-com-pricing-api-openapi.yml
  format: yaml
  label: CostBench Pricing API
  slug: costbench-com-pricing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/costbench-com/openapi/costbench-com-pricing-api-openapi.yml
- filename: costbench-com-tco-api-openapi.yml
  format: yaml
  label: CostBench Tco API
  slug: costbench-com-tco-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/costbench-com/openapi/costbench-com-tco-api-openapi.yml
- filename: costbench-com-usage-api-openapi.yml
  format: yaml
  label: CostBench Usage API
  slug: costbench-com-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/costbench-com/openapi/costbench-com-usage-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: costbench.com
  spf: true
hosts:
- cert_expires: Dec 15 23:34:42 2026 GMT
  host: costbench.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: CostBench Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CostBench, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: CostBench
provider_slug: costbench-com
slug: costbench-com-domain-security
source_filename: costbench-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: costbench.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 23:34:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: costbench.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/costbench-com/security/costbench-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Software Pricing
- Software-as-a-Service
- Procurement
- Cost Intelligence
- Price Comparison
- Total Cost of Ownership
- MCP
---
