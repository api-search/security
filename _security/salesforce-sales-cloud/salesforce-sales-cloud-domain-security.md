---
api_specs:
- filename: salesforce-sales-cloud-rest-api-openapi.yml
  format: yaml
  label: Salesforce REST API
  slug: salesforce-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-sales-cloud/refs/heads/main/openapi/salesforce-sales-cloud-rest-api-openapi.yml
- filename: salesforce-sales-cloud-bulk-api-openapi.yml
  format: yaml
  label: Bulk API 2.0
  slug: bulk-api-20
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-sales-cloud/refs/heads/main/openapi/salesforce-sales-cloud-bulk-api-openapi.yml
- filename: salesforce-sales-cloud-platform-events-api-openapi.yml
  format: yaml
  label: Platform Events API
  slug: platform-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-sales-cloud/refs/heads/main/openapi/salesforce-sales-cloud-platform-events-api-openapi.yml
- filename: salesforce-sales-cloud-analytics-api-openapi.yml
  format: yaml
  label: Analytics REST API
  slug: analytics-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-sales-cloud/refs/heads/main/openapi/salesforce-sales-cloud-analytics-api-openapi.yml
- filename: salesforce-sales-cloud-composite-api-openapi.yml
  format: yaml
  label: Salesforce Composite API
  slug: salesforce-composite-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-sales-cloud/refs/heads/main/openapi/salesforce-sales-cloud-composite-api-openapi.yml
- filename: salesforce-sales-cloud-graphql-api-openapi.yml
  format: yaml
  label: Salesforce GraphQL API
  slug: salesforce-graphql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-sales-cloud/refs/heads/main/openapi/salesforce-sales-cloud-graphql-api-openapi.yml
- filename: salesforce-sales-cloud-tooling-api-openapi.yml
  format: yaml
  label: Salesforce Tooling API
  slug: salesforce-tooling-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-sales-cloud/refs/heads/main/openapi/salesforce-sales-cloud-tooling-api-openapi.yml
- filename: salesforce-sales-cloud-change-data-capture-api-openapi.yml
  format: yaml
  label: Salesforce Change Data Capture API
  slug: salesforce-change-data-capture-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-sales-cloud/refs/heads/main/openapi/salesforce-sales-cloud-change-data-capture-api-openapi.yml
- filename: salesforce-sales-cloud-connect-api-openapi.yml
  format: yaml
  label: Salesforce Connect REST API
  slug: salesforce-connect-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-sales-cloud/refs/heads/main/openapi/salesforce-sales-cloud-connect-api-openapi.yml
- filename: salesforce-sales-cloud-ui-api-openapi.yml
  format: yaml
  label: Salesforce User Interface API
  slug: salesforce-user-interface-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-sales-cloud/refs/heads/main/openapi/salesforce-sales-cloud-ui-api-openapi.yml
- filename: salesforce-sales-cloud-apex-rest-api-openapi.yml
  format: yaml
  label: Salesforce Apex REST API
  slug: salesforce-apex-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-sales-cloud/refs/heads/main/openapi/salesforce-sales-cloud-apex-rest-api-openapi.yml
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
name: Salesforce Sales Cloud Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Salesforce Sales Cloud, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Salesforce Sales Cloud
provider_slug: salesforce-sales-cloud
slug: salesforce-sales-cloud-domain-security
source_filename: salesforce-sales-cloud-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.salesforce.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 23:59:59 2026 GMT\n  hsts: null\n- host: www.salesforce.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 86400\n- host: yourinstance.salesforce.com\n  https: false\ndomains:\n- domain: salesforce.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/salesforce-sales-cloud/refs/heads/main/security/salesforce-sales-cloud-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Cloud
- CRM
- Customer Management
- Enterprise
- Sales
---
