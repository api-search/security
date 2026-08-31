---
api_specs:
- filename: immuta-access-request-api-openapi.yml
  format: yaml
  label: Immuta Access Request API
  slug: immuta-access-request-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/immuta/refs/heads/main/openapi/immuta-access-request-api-openapi.yml
- filename: immuta-asset-api-openapi.yml
  format: yaml
  label: Immuta Asset API
  slug: immuta-asset-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/immuta/refs/heads/main/openapi/immuta-asset-api-openapi.yml
- filename: immuta-auth-api-openapi.yml
  format: yaml
  label: Immuta Auth API
  slug: immuta-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/immuta/refs/heads/main/openapi/immuta-auth-api-openapi.yml
- filename: immuta-data-product-api-openapi.yml
  format: yaml
  label: Immuta Data Product API
  slug: immuta-data-product-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/immuta/refs/heads/main/openapi/immuta-data-product-api-openapi.yml
- filename: immuta-data-source-api-openapi.yml
  format: yaml
  label: Immuta Data Source API
  slug: immuta-data-source-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/immuta/refs/heads/main/openapi/immuta-data-source-api-openapi.yml
- filename: immuta-data-use-agreement-api-openapi.yml
  format: yaml
  label: Immuta Data Use Agreement API
  slug: immuta-data-use-agreement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/immuta/refs/heads/main/openapi/immuta-data-use-agreement-api-openapi.yml
- filename: immuta-health-api-openapi.yml
  format: yaml
  label: Immuta Health API
  slug: immuta-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/immuta/refs/heads/main/openapi/immuta-health-api-openapi.yml
- filename: immuta-metadata-api-openapi.yml
  format: yaml
  label: Immuta Metadata API
  slug: immuta-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/immuta/refs/heads/main/openapi/immuta-metadata-api-openapi.yml
- filename: immuta-notification-api-openapi.yml
  format: yaml
  label: Immuta Notification API
  slug: immuta-notification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/immuta/refs/heads/main/openapi/immuta-notification-api-openapi.yml
- filename: immuta-request-form-api-openapi.yml
  format: yaml
  label: Immuta Request Form API
  slug: immuta-request-form-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/immuta/refs/heads/main/openapi/immuta-request-form-api-openapi.yml
- filename: immuta-settings-api-openapi.yml
  format: yaml
  label: Immuta Settings API
  slug: immuta-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/immuta/refs/heads/main/openapi/immuta-settings-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: immuta.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: immutacloud.com
  spf: false
hosts:
- cert_expires: Sep 16 01:01:50 2026 GMT
  host: www.immuta.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 17:41:15 2026 GMT
  host: documentation.immuta.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 19 22:57:53 2026 GMT
  host: na.api.immutacloud.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Immuta Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Immuta, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Immuta
provider_slug: immuta
slug: immuta-domain-security
source_filename: immuta-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.immuta.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 01:01:50 2026 GMT\n  hsts: false\n- host: documentation.immuta.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 17:41:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: na.api.immutacloud.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 22:57:53 2026 GMT\n  hsts: null\ndomains:\n- domain: immuta.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: immutacloud.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/immuta/refs/heads/main/security/immuta-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Data Governance
- Data Access Control
- Data Security
- Data Privacy
- Policy Management
- Data Marketplace
- Compliance
- Snowflake
- Databricks
- Analytics
- Agentic Data Access
---
