---
api_specs:
- filename: widen-acquia-dam-webhooks-api-openapi.yml
  format: yaml
  label: Widen Acquia-DAM-Webhooks API
  slug: widen-acquia-dam-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/widen/refs/heads/main/openapi/widen-acquia-dam-webhooks-api-openapi.yml
- filename: widen-analytics-api-openapi.yml
  format: yaml
  label: Widen Analytics API
  slug: widen-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/widen/refs/heads/main/openapi/widen-analytics-api-openapi.yml
- filename: widen-assets-api-openapi.yml
  format: yaml
  label: Widen Assets API
  slug: widen-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/widen/refs/heads/main/openapi/widen-assets-api-openapi.yml
- filename: widen-attributes-api-openapi.yml
  format: yaml
  label: Widen Attributes API
  slug: widen-attributes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/widen/refs/heads/main/openapi/widen-attributes-api-openapi.yml
- filename: widen-categories-api-openapi.yml
  format: yaml
  label: Widen Categories API
  slug: widen-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/widen/refs/heads/main/openapi/widen-categories-api-openapi.yml
- filename: widen-channels-api-openapi.yml
  format: yaml
  label: Widen Channels API
  slug: widen-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/widen/refs/heads/main/openapi/widen-channels-api-openapi.yml
- filename: widen-collections-api-openapi.yml
  format: yaml
  label: Widen Collections API
  slug: widen-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/widen/refs/heads/main/openapi/widen-collections-api-openapi.yml
- filename: widen-file-formats-api-openapi.yml
  format: yaml
  label: Widen File-Formats API
  slug: widen-file-formats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/widen/refs/heads/main/openapi/widen-file-formats-api-openapi.yml
- filename: widen-integration-links-api-openapi.yml
  format: yaml
  label: Widen Integration-Links API
  slug: widen-integration-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/widen/refs/heads/main/openapi/widen-integration-links-api-openapi.yml
- filename: widen-metadata-api-openapi.yml
  format: yaml
  label: Widen Metadata API
  slug: widen-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/widen/refs/heads/main/openapi/widen-metadata-api-openapi.yml
- filename: widen-orders-api-openapi.yml
  format: yaml
  label: Widen Orders API
  slug: widen-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/widen/refs/heads/main/openapi/widen-orders-api-openapi.yml
- filename: widen-products-api-openapi.yml
  format: yaml
  label: Widen Products API
  slug: widen-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/widen/refs/heads/main/openapi/widen-products-api-openapi.yml
- filename: widen-search-connector-api-openapi.yml
  format: yaml
  label: Widen Search-Connector API
  slug: widen-search-connector-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/widen/refs/heads/main/openapi/widen-search-connector-api-openapi.yml
- filename: widen-usage-api-openapi.yml
  format: yaml
  label: Widen Usage API
  slug: widen-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/widen/refs/heads/main/openapi/widen-usage-api-openapi.yml
- filename: widen-users-api-openapi.yml
  format: yaml
  label: Widen Users API
  slug: widen-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/widen/refs/heads/main/openapi/widen-users-api-openapi.yml
- filename: widen-workflow-app-projects-api-openapi.yml
  format: yaml
  label: Widen Workflow-App-Projects API
  slug: widen-workflow-app-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/widen/refs/heads/main/openapi/widen-workflow-app-projects-api-openapi.yml
- filename: widen-workflow-webhooks-api-openapi.yml
  format: yaml
  label: Widen Workflow-Webhooks API
  slug: widen-workflow-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/widen/refs/heads/main/openapi/widen-workflow-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: acquia.com
  spf: true
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: widencollective.com
  spf: true
hosts:
- cert_expires: Nov  7 23:59:59 2026 GMT
  host: www.acquia.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Nov  7 23:59:59 2026 GMT
  host: docs.acquia.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Feb 16 23:59:59 2027 GMT
  host: api.widencollective.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Widen Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Widen, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Widen
provider_slug: widen
slug: widen-domain-security
source_filename: widen-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.acquia.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  7 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.acquia.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  7 23:59:59 2026 GMT\n  hsts: false\n- host: api.widencollective.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 16 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: acquia.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: widencollective.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/widen/refs/heads/main/security/widen-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC · DMARC
tags:
- Digital Asset Management
- DAM
- Media
- Assets
- Metadata
- Collection
- Workflows
- Acquia
---
