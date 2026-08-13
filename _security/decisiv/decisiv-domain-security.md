---
api_specs:
- filename: decisiv-account-management-openapi.yml
  format: yaml
  label: Decisiv SRM Gateway - Account Management
  slug: decisiv-srm-gateway-account-management
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/decisiv/refs/heads/main/openapi/decisiv-account-management-openapi.yml
- filename: decisiv-asset-management-openapi.yml
  format: yaml
  label: Decisiv SRM Gateway - Asset Management
  slug: decisiv-srm-gateway-asset-management
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/decisiv/refs/heads/main/openapi/decisiv-asset-management-openapi.yml
- filename: decisiv-service-management-openapi.yml
  format: yaml
  label: Decisiv SRM Gateway - Service Management
  slug: decisiv-srm-gateway-service-management
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/decisiv/refs/heads/main/openapi/decisiv-service-management-openapi.yml
- filename: decisiv-telematics-openapi.yml
  format: yaml
  label: Decisiv SRM Gateway - Telematics
  slug: decisiv-srm-gateway-telematics
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/decisiv/refs/heads/main/openapi/decisiv-telematics-openapi.yml
- filename: decisiv-global-assets-openapi.yml
  format: yaml
  label: Decisiv Global Assets API
  slug: decisiv-global-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/decisiv/refs/heads/main/openapi/decisiv-global-assets-openapi.yml
- filename: decisiv-service-provider-openapi.yml
  format: yaml
  label: Decisiv Service Provider API
  slug: decisiv-service-provider-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/decisiv/refs/heads/main/openapi/decisiv-service-provider-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: decisiv.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: decisivapps.com
  spf: true
hosts:
- cert_expires: Oct 31 05:30:42 2026 GMT
  host: www.decisiv.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 20 23:59:59 2026 GMT
  host: srm-api.decisivapps.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  6 23:59:59 2027 GMT
  host: global-assets.decisivapps.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Decisiv Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Decisiv, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Decisiv
provider_slug: decisiv
slug: decisiv-domain-security
source_filename: decisiv-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.decisiv.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 31 05:30:42 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: srm-api.decisivapps.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 23:59:59 2026 GMT\n  hsts: null\n- host: global-assets.decisivapps.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  6 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: decisiv.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: decisivapps.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/decisiv/refs/heads/main/security/decisiv-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- commercial-vehicle
- fleet-management
- service-relationship-management
- telematics
- asset-management
- maintenance-and-repair
- heavy-duty-trucking
- transportation
- dealer-management
- json-api
- webhooks
---
