---
api_specs:
- filename: amobee-env-vars-test-controller-api-openapi.yml
  format: yaml
  label: Amobee Env Vars Test Controller API
  slug: amobee-env-vars-test-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amobee/refs/heads/main/openapi/amobee-env-vars-test-controller-api-openapi.yml
- filename: amobee-gateway-swagger-controller-api-openapi.yml
  format: yaml
  label: Amobee Gateway Swagger Controller API
  slug: amobee-gateway-swagger-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amobee/refs/heads/main/openapi/amobee-gateway-swagger-controller-api-openapi.yml
- filename: amobee-health-check-api-openapi.yml
  format: yaml
  label: Amobee Health Check API
  slug: amobee-health-check-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amobee/refs/heads/main/openapi/amobee-health-check-api-openapi.yml
- filename: amobee-ip-controller-api-openapi.yml
  format: yaml
  label: Amobee Ip Controller API
  slug: amobee-ip-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amobee/refs/heads/main/openapi/amobee-ip-controller-api-openapi.yml
- filename: amobee-tcf-disclosure-controller-api-openapi.yml
  format: yaml
  label: Amobee Tcf Disclosure Controller API
  slug: amobee-tcf-disclosure-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amobee/refs/heads/main/openapi/amobee-tcf-disclosure-controller-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: amobee.com
  spf: true
hosts:
- cert_expires: Oct 19 06:29:28 2026 GMT
  host: www.amobee.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 16 23:59:59 2026 GMT
  host: services.amobee.com
  hsts: null
  hsts_note: 'The root path returns a bare JSON 404 without HSTS, but the live API paths do send it — https://services.amobee.com/accounts/v1/api/token returned ''strict-transport-security: max-age=15724800; includeSubDomains'' on 2026-08-12, along with x-content-type-options, x-frame-options, referrer-policy, permissions-policy and a Content-Security-Policy.'
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Amobee Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amobee, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Amobee
provider_slug: amobee
slug: amobee-domain-security
source_filename: amobee-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.amobee.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 06:29:28 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: services.amobee.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 23:59:59 2026 GMT\n  hsts: null\n  hsts_note: >-\n    The root path returns a bare JSON 404 without HSTS, but the live API paths do\n    send it — https://services.amobee.com/accounts/v1/api/token returned\n    'strict-transport-security: max-age=15724800; includeSubDomains' on 2026-08-12,\n    along with x-content-type-options, x-frame-options, referrer-policy,\n    permissions-policy and a Content-Security-Policy.\ndomains:\n- domain: amobee.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amobee/refs/heads/main/security/amobee-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Digital Advertising
- DSP
- Programmatic
- Campaign Management
- Audience Targeting
- Data Management Platform
- AdTech
- Samsung Ads
---
