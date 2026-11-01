---
api_specs:
- filename: ampersand-api-key-api-openapi.yml
  format: yaml
  label: Ampersand API Key API
  slug: ampersand-api-key-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ampersand/openapi/ampersand-api-key-api-openapi.yml
- filename: ampersand-billing-account-api-openapi.yml
  format: yaml
  label: Ampersand Billing Account API
  slug: ampersand-billing-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ampersand/openapi/ampersand-billing-account-api-openapi.yml
- filename: ampersand-connection-api-openapi.yml
  format: yaml
  label: Ampersand Connection API
  slug: ampersand-connection-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ampersand/openapi/ampersand-connection-api-openapi.yml
- filename: ampersand-destination-api-openapi.yml
  format: yaml
  label: Ampersand Destination API
  slug: ampersand-destination-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ampersand/openapi/ampersand-destination-api-openapi.yml
- filename: ampersand-installation-api-openapi.yml
  format: yaml
  label: Ampersand Installation API
  slug: ampersand-installation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ampersand/openapi/ampersand-installation-api-openapi.yml
- filename: ampersand-integration-api-openapi.yml
  format: yaml
  label: Ampersand Integration API
  slug: ampersand-integration-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ampersand/openapi/ampersand-integration-api-openapi.yml
- filename: ampersand-jwt-key-api-openapi.yml
  format: yaml
  label: Ampersand JWT Key API
  slug: ampersand-jwt-key-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ampersand/openapi/ampersand-jwt-key-api-openapi.yml
- filename: ampersand-notification-api-openapi.yml
  format: yaml
  label: Ampersand Notification API
  slug: ampersand-notification-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ampersand/openapi/ampersand-notification-api-openapi.yml
- filename: ampersand-oauth-api-openapi.yml
  format: yaml
  label: Ampersand OAuth API
  slug: ampersand-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ampersand/openapi/ampersand-oauth-api-openapi.yml
- filename: ampersand-objects-fields-api-openapi.yml
  format: yaml
  label: Ampersand Objects & Fields API
  slug: ampersand-objects-fields-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ampersand/openapi/ampersand-objects-fields-api-openapi.yml
- filename: ampersand-operation-api-openapi.yml
  format: yaml
  label: Ampersand Operation API
  slug: ampersand-operation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ampersand/openapi/ampersand-operation-api-openapi.yml
- filename: ampersand-org-api-openapi.yml
  format: yaml
  label: Ampersand Org API
  slug: ampersand-org-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ampersand/openapi/ampersand-org-api-openapi.yml
- filename: ampersand-project-api-openapi.yml
  format: yaml
  label: Ampersand Project API
  slug: ampersand-project-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ampersand/openapi/ampersand-project-api-openapi.yml
- filename: ampersand-provider-api-openapi.yml
  format: yaml
  label: Ampersand Provider API
  slug: ampersand-provider-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ampersand/openapi/ampersand-provider-api-openapi.yml
- filename: ampersand-provider-app-api-openapi.yml
  format: yaml
  label: Ampersand Provider App API
  slug: ampersand-provider-app-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ampersand/openapi/ampersand-provider-app-api-openapi.yml
- filename: ampersand-revision-api-openapi.yml
  format: yaml
  label: Ampersand Revision API
  slug: ampersand-revision-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ampersand/openapi/ampersand-revision-api-openapi.yml
- filename: ampersand-upload-url-api-openapi.yml
  format: yaml
  label: Ampersand Upload URL API
  slug: ampersand-upload-url-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ampersand/openapi/ampersand-upload-url-api-openapi.yml
- filename: ampersand-user-api-openapi.yml
  format: yaml
  label: Ampersand User API
  slug: ampersand-user-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ampersand/openapi/ampersand-user-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: withampersand.com
  spf: true
hosts:
- cert_expires: Oct  5 16:05:56 2026 GMT
  host: www.withampersand.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 17:13:55 2026 GMT
  host: docs.withampersand.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 19:38:48 2026 GMT
  host: api.withampersand.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Ampersand Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ampersand, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Ampersand
provider_slug: ampersand
slug: ampersand-domain-security
source_filename: ampersand-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.withampersand.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 16:05:56 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.withampersand.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 17:13:55 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.withampersand.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 19:38:48 2026 GMT\n  hsts: null\ndomains:\n- domain: withampersand.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/ampersand/security/ampersand-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Developer Tools
- Integration
- Platform
- Software-as-a-Service
- Authentication
- Data Sync
- Webhook
---
