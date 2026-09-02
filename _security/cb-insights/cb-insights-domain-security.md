---
api_specs:
- filename: cb-insights-authorization-api-openapi.yml
  format: yaml
  label: CB Insights Authorization API
  slug: cb-insights-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cb-insights/refs/heads/main/openapi/cb-insights-authorization-api-openapi.yml
- filename: cb-insights-businessrelationships-api-openapi.yml
  format: yaml
  label: CB Insights Business Relationships API
  slug: cb-insights-businessrelationships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cb-insights/refs/heads/main/openapi/cb-insights-businessrelationships-api-openapi.yml
- filename: cb-insights-chatcbi-api-openapi.yml
  format: yaml
  label: CB Insights Chat CBI API
  slug: cb-insights-chatcbi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cb-insights/refs/heads/main/openapi/cb-insights-chatcbi-api-openapi.yml
- filename: cb-insights-financialtransactions-api-openapi.yml
  format: yaml
  label: CB Insights Financial Transactions API
  slug: cb-insights-financialtransactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cb-insights/refs/heads/main/openapi/cb-insights-financialtransactions-api-openapi.yml
- filename: cb-insights-firmographics-api-openapi.yml
  format: yaml
  label: CB Insights Firmographics API
  slug: cb-insights-firmographics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cb-insights/refs/heads/main/openapi/cb-insights-firmographics-api-openapi.yml
- filename: cb-insights-managementandboard-api-openapi.yml
  format: yaml
  label: CB Insights Management And Board API
  slug: cb-insights-managementandboard-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cb-insights/refs/heads/main/openapi/cb-insights-managementandboard-api-openapi.yml
- filename: cb-insights-organizations-api-openapi.yml
  format: yaml
  label: CB Insights Organizations API
  slug: cb-insights-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cb-insights/refs/heads/main/openapi/cb-insights-organizations-api-openapi.yml
- filename: cb-insights-outlook-api-openapi.yml
  format: yaml
  label: CB Insights Outlook API
  slug: cb-insights-outlook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cb-insights/refs/heads/main/openapi/cb-insights-outlook-api-openapi.yml
- filename: cb-insights-revenue-api-openapi.yml
  format: yaml
  label: CB Insights Revenue API
  slug: cb-insights-revenue-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cb-insights/refs/heads/main/openapi/cb-insights-revenue-api-openapi.yml
- filename: cb-insights-scoutingreports-api-openapi.yml
  format: yaml
  label: CB Insights Scouting Reports API
  slug: cb-insights-scoutingreports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cb-insights/refs/heads/main/openapi/cb-insights-scoutingreports-api-openapi.yml
- filename: cb-insights-strategymap-api-openapi.yml
  format: yaml
  label: CB Insights Strategy Map API
  slug: cb-insights-strategymap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cb-insights/refs/heads/main/openapi/cb-insights-strategymap-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cbinsights.com
  spf: true
hosts:
- cert_expires: Jan 14 23:59:59 2027 GMT
  host: www.cbinsights.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 14 23:59:59 2027 GMT
  host: api-docs.cbinsights.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 20 23:59:59 2027 GMT
  host: api.cbinsights.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 20 23:59:59 2027 GMT
  host: mcp.cbinsights.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  note: The only host in the estate that sets Strict-Transport-Security. Probed 2026-08-09; GET returns 405 Method Not Allowed (POST-only MCP endpoint) with the HSTS header present on the 405.
  server: envoy
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cb Insights Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CB Insights, probed live across 4 host(s) and 1 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: CB Insights
provider_slug: cb-insights
slug: cb-insights-domain-security
source_filename: cb-insights-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cbinsights.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 23:59:59 2027 GMT\n  hsts: false\n- host: api-docs.cbinsights.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 23:59:59 2027 GMT\n  hsts: false\n- host: api.cbinsights.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 23:59:59 2027 GMT\n  hsts: null\n- host: mcp.cbinsights.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  server: envoy\n  note: >-\n    The only host in the estate that sets Strict-Transport-Security. Probed 2026-08-09; GET returns\n    405 Method Not Allowed (POST-only MCP endpoint) with the HSTS header present on the 405.\ndomains:\n- domain: cbinsights.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cb-insights/refs/heads/main/security/cb-insights-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Market Intelligence
- private-company-data
- Venture Capital
- Funding Data
- investor-data
- Company Data
- People Data
- BusinessRelationships
- predictive-scoring
- MCP
- agent-native
- Data Enrichment
- Snowflake
---
