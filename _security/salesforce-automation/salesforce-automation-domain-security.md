---
api_specs:
- filename: salesforce-rest-api-openapi.json
  format: json
  label: Salesforce REST API
  slug: salesforce-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-automation/refs/heads/main/openapi/salesforce-rest-api-openapi.json
- filename: salesforce-bulk-api-openapi.json
  format: json
  label: Salesforce Bulk API 2.0
  slug: salesforce-bulk-api-20
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-automation/refs/heads/main/openapi/salesforce-bulk-api-openapi.json
- filename: salesforce-streaming-api-openapi.json
  format: json
  label: Salesforce Streaming API
  slug: salesforce-streaming-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-automation/refs/heads/main/openapi/salesforce-streaming-api-openapi.json
- filename: salesforce-platform-events-api-openapi.json
  format: json
  label: Salesforce Platform Events API
  slug: salesforce-platform-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-automation/refs/heads/main/openapi/salesforce-platform-events-api-openapi.json
- filename: salesforce-analytics-api-openapi.json
  format: json
  label: Salesforce Analytics API
  slug: salesforce-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-automation/refs/heads/main/openapi/salesforce-analytics-api-openapi.json
- filename: salesforce-tooling-api-openapi.json
  format: json
  label: Salesforce Tooling API
  slug: salesforce-tooling-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-automation/refs/heads/main/openapi/salesforce-tooling-api-openapi.json
- filename: salesforce-connect-rest-api-openapi.json
  format: json
  label: Salesforce Connect REST API
  slug: salesforce-connect-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-automation/refs/heads/main/openapi/salesforce-connect-rest-api-openapi.json
- filename: salesforce-change-data-capture-api-openapi.json
  format: json
  label: Salesforce Change Data Capture API
  slug: salesforce-change-data-capture-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-automation/refs/heads/main/openapi/salesforce-change-data-capture-api-openapi.json
- filename: salesforce-invocable-actions-api-openapi.json
  format: json
  label: Salesforce Invocable Actions API
  slug: salesforce-invocable-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-automation/refs/heads/main/openapi/salesforce-invocable-actions-api-openapi.json
- filename: salesforce-composite-api-openapi.json
  format: json
  label: Salesforce Composite API
  slug: salesforce-composite-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-automation/refs/heads/main/openapi/salesforce-composite-api-openapi.json
- filename: salesforce-apex-rest-api-openapi.json
  format: json
  label: Salesforce Apex REST API
  slug: salesforce-apex-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-automation/refs/heads/main/openapi/salesforce-apex-rest-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: salesforce.com
  spf: true
hosts:
- cert_expires: Oct 10 23:59:59 2026 GMT
  host: developer.salesforce.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 23:59:59 2026 GMT
  host: www.salesforce.com
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
- host: yourinstance.salesforce.com
  https: false
kind: domain-security
layout: security
method: probed
name: Salesforce Automation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Salesforce Automation, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Salesforce Automation
provider_slug: salesforce-automation
slug: salesforce-automation-domain-security
source_filename: salesforce-automation-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.salesforce.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 23:59:59 2026 GMT\n  hsts: null\n- host: www.salesforce.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 86400\n- host: yourinstance.salesforce.com\n  https: false\ndomains:\n- domain: salesforce.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/salesforce-automation/refs/heads/main/security/salesforce-automation-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Automation
- Cloud
- CRM
- Enterprise
- Sales
---
