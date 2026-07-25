---
api_specs:
- filename: salesforce-streaming-api-asyncapi.yml
  format: yaml
  label: Service Cloud Streaming API
  slug: service-cloud-streaming-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-service-cloud/refs/heads/main/asyncapi/salesforce-streaming-api-asyncapi.yml
- filename: salesforce-service-cloud-accounts-api-openapi.yml
  format: yaml
  label: Salesforce Service Cloud Accounts API
  slug: salesforce-service-cloud-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-service-cloud/refs/heads/main/openapi/salesforce-service-cloud-accounts-api-openapi.yml
- filename: salesforce-service-cloud-availability-api-openapi.yml
  format: yaml
  label: Salesforce Service Cloud Availability API
  slug: salesforce-service-cloud-availability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-service-cloud/refs/heads/main/openapi/salesforce-service-cloud-availability-api-openapi.yml
- filename: salesforce-service-cloud-cases-api-openapi.yml
  format: yaml
  label: Salesforce Service Cloud Cases API
  slug: salesforce-service-cloud-cases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-service-cloud/refs/heads/main/openapi/salesforce-service-cloud-cases-api-openapi.yml
- filename: salesforce-service-cloud-contacts-api-openapi.yml
  format: yaml
  label: Salesforce Service Cloud Contacts API
  slug: salesforce-service-cloud-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-service-cloud/refs/heads/main/openapi/salesforce-service-cloud-contacts-api-openapi.yml
- filename: salesforce-service-cloud-knowledge-api-openapi.yml
  format: yaml
  label: Salesforce Service Cloud Knowledge API
  slug: salesforce-service-cloud-knowledge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-service-cloud/refs/heads/main/openapi/salesforce-service-cloud-knowledge-api-openapi.yml
- filename: salesforce-service-cloud-messages-api-openapi.yml
  format: yaml
  label: Salesforce Service Cloud Messages API
  slug: salesforce-service-cloud-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-service-cloud/refs/heads/main/openapi/salesforce-service-cloud-messages-api-openapi.yml
- filename: salesforce-service-cloud-query-api-openapi.yml
  format: yaml
  label: Salesforce Service Cloud Query API
  slug: salesforce-service-cloud-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-service-cloud/refs/heads/main/openapi/salesforce-service-cloud-query-api-openapi.yml
- filename: salesforce-service-cloud-search-api-openapi.yml
  format: yaml
  label: Salesforce Service Cloud Search API
  slug: salesforce-service-cloud-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-service-cloud/refs/heads/main/openapi/salesforce-service-cloud-search-api-openapi.yml
- filename: salesforce-service-cloud-sessions-api-openapi.yml
  format: yaml
  label: Salesforce Service Cloud Sessions API
  slug: salesforce-service-cloud-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-service-cloud/refs/heads/main/openapi/salesforce-service-cloud-sessions-api-openapi.yml
- filename: salesforce-service-cloud-settings-api-openapi.yml
  format: yaml
  label: Salesforce Service Cloud Settings API
  slug: salesforce-service-cloud-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-service-cloud/refs/heads/main/openapi/salesforce-service-cloud-settings-api-openapi.yml
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
- host: yourinstance.salesforce.com
  https: false
kind: domain-security
layout: security
method: probed
name: Salesforce Service Cloud Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Salesforce Service Cloud, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Salesforce Service Cloud
provider_slug: salesforce-service-cloud
slug: salesforce-service-cloud-domain-security
source_filename: salesforce-service-cloud-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.salesforce.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 23:59:59 2026 GMT\n  hsts: null\n- host: yourinstance.salesforce.com\n  https: false\ndomains:\n- domain: salesforce.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/salesforce-service-cloud/refs/heads/main/security/salesforce-service-cloud-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Case Management
- CRM
- Customer Service
- Help Desk
- Support
- Ticketing
---
