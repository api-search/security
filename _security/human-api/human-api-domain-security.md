---
api_specs:
- filename: human-api-admin-api-openapi.yml
  format: yaml
  label: Human API Admin API
  slug: human-api-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/human-api/refs/heads/main/openapi/human-api-admin-api-openapi.yml
- filename: human-api-connect-api-openapi.yml
  format: yaml
  label: Human API Connect API
  slug: human-api-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/human-api/refs/heads/main/openapi/human-api-connect-api-openapi.yml
- filename: human-api-orders-api-openapi.yml
  format: yaml
  label: Human API Orders API
  slug: human-api-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/human-api/refs/heads/main/openapi/human-api-orders-api-openapi.yml
- filename: human-api-reports-api-openapi.yml
  format: yaml
  label: Human API Reports API
  slug: human-api-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/human-api/refs/heads/main/openapi/human-api-reports-api-openapi.yml
- filename: human-api-resources-api-openapi.yml
  format: yaml
  label: Human API Resources API
  slug: human-api-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/human-api/refs/heads/main/openapi/human-api-resources-api-openapi.yml
- filename: human-api-subscriptions-api-openapi.yml
  format: yaml
  label: Human API Subscriptions API
  slug: human-api-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/human-api/refs/heads/main/openapi/human-api-subscriptions-api-openapi.yml
- filename: human-api-users-api-openapi.yml
  format: yaml
  label: Human API Users API
  slug: human-api-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/human-api/refs/heads/main/openapi/human-api-users-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: humanapi.co
  spf: true
hosts:
- cert_expires: Dec 26 20:36:25 2026 GMT
  host: humanapi.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 13:10:17 2026 GMT
  host: reference.humanapi.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  6 23:59:59 2026 GMT
  host: admin.humanapi.co
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Human Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Human API, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Human API
provider_slug: human-api
slug: human-api-domain-security
source_filename: human-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: humanapi.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 20:36:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: reference.humanapi.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 13:10:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: admin.humanapi.co\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  6 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: humanapi.co\n  dnssec: false\n  caa:\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/human-api/refs/heads/main/security/human-api-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Healthcare
- United States
- Health Data
- EHR
- Interoperability
- Remote Monitoring
- Wearables
- Life Insurance
- Clinical Data
- Health API
---
