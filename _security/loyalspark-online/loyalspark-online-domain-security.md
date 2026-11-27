---
api_specs:
- filename: loyalspark-online-billing-api-openapi.yml
  format: yaml
  label: Loyal Spark Billing API
  slug: loyalspark-online-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/loyalspark-online/openapi/loyalspark-online-billing-api-openapi.yml
- filename: loyalspark-online-identity-api-openapi.yml
  format: yaml
  label: Loyal Spark Identity API
  slug: loyalspark-online-identity-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/loyalspark-online/openapi/loyalspark-online-identity-api-openapi.yml
- filename: loyalspark-online-merchant-mcp-api-openapi.yml
  format: yaml
  label: Loyal Spark Merchant MCP API
  slug: loyalspark-online-merchant-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/loyalspark-online/openapi/loyalspark-online-merchant-mcp-api-openapi.yml
- filename: loyalspark-online-merchant-rest-api-openapi.yml
  format: yaml
  label: Loyal Spark Merchant REST API
  slug: loyalspark-online-merchant-rest-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/loyalspark-online/openapi/loyalspark-online-merchant-rest-api-openapi.yml
- filename: loyalspark-online-recipient-mcp-api-openapi.yml
  format: yaml
  label: Loyal Spark Recipient MCP API
  slug: loyalspark-online-recipient-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/loyalspark-online/openapi/loyalspark-online-recipient-mcp-api-openapi.yml
- filename: loyalspark-online-recipient-rest-api-openapi.yml
  format: yaml
  label: Loyal Spark Recipient REST API
  slug: loyalspark-online-recipient-rest-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/loyalspark-online/openapi/loyalspark-online-recipient-rest-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: loyalspark.online
  spf: true
hosts:
- cert_expires: Jan  5 12:44:56 2027 GMT
  host: loyalspark.online
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Loyal Spark Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Loyal Spark, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Loyal Spark
provider_slug: loyalspark-online
slug: loyalspark-online-domain-security
source_filename: loyalspark-online-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: loyalspark.online\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 12:44:56 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: loyalspark.online\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/loyalspark-online/security/loyalspark-online-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Loyalty
- Blockchain
- Rewards
- Artificial Intelligence
- Payments
---
