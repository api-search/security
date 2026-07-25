---
api_specs:
- filename: appcues-banners-api-openapi.yml
  format: yaml
  label: Appcues Banners API
  slug: appcues-banners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appcues/refs/heads/main/openapi/appcues-banners-api-openapi.yml
- filename: appcues-events-api-openapi.yml
  format: yaml
  label: Appcues Events API
  slug: appcues-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appcues/refs/heads/main/openapi/appcues-events-api-openapi.yml
- filename: appcues-exports-api-openapi.yml
  format: yaml
  label: Appcues Exports API
  slug: appcues-exports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appcues/refs/heads/main/openapi/appcues-exports-api-openapi.yml
- filename: appcues-flows-api-openapi.yml
  format: yaml
  label: Appcues Flows API
  slug: appcues-flows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appcues/refs/heads/main/openapi/appcues-flows-api-openapi.yml
- filename: appcues-groups-api-openapi.yml
  format: yaml
  label: Appcues Groups API
  slug: appcues-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appcues/refs/heads/main/openapi/appcues-groups-api-openapi.yml
- filename: appcues-imports-api-openapi.yml
  format: yaml
  label: Appcues Imports API
  slug: appcues-imports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appcues/refs/heads/main/openapi/appcues-imports-api-openapi.yml
- filename: appcues-jobs-api-openapi.yml
  format: yaml
  label: Appcues Jobs API
  slug: appcues-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appcues/refs/heads/main/openapi/appcues-jobs-api-openapi.yml
- filename: appcues-launchpads-api-openapi.yml
  format: yaml
  label: Appcues Launchpads API
  slug: appcues-launchpads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appcues/refs/heads/main/openapi/appcues-launchpads-api-openapi.yml
- filename: appcues-mobile-api-openapi.yml
  format: yaml
  label: Appcues Mobile API
  slug: appcues-mobile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appcues/refs/heads/main/openapi/appcues-mobile-api-openapi.yml
- filename: appcues-pins-api-openapi.yml
  format: yaml
  label: Appcues Pins API
  slug: appcues-pins-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appcues/refs/heads/main/openapi/appcues-pins-api-openapi.yml
- filename: appcues-segments-api-openapi.yml
  format: yaml
  label: Appcues Segments API
  slug: appcues-segments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appcues/refs/heads/main/openapi/appcues-segments-api-openapi.yml
- filename: appcues-tags-api-openapi.yml
  format: yaml
  label: Appcues Tags API
  slug: appcues-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appcues/refs/heads/main/openapi/appcues-tags-api-openapi.yml
- filename: appcues-users-api-openapi.yml
  format: yaml
  label: Appcues Users API
  slug: appcues-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appcues/refs/heads/main/openapi/appcues-users-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: appcues.com
  spf: true
hosts:
- cert_expires: Oct  3 01:45:28 2026 GMT
  host: www.appcues.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 23:59:59 2026 GMT
  host: api.appcues.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Jan 10 23:59:59 2027 GMT
  host: api.eu.appcues.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Appcues Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Appcues, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Appcues
provider_slug: appcues
slug: appcues-domain-security
source_filename: appcues-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.appcues.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 01:45:28 2026 GMT\n  hsts: false\n- host: api.appcues.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 15 23:59:59 2026 GMT\n  hsts: false\n- host: api.eu.appcues.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 10 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: appcues.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/appcues/refs/heads/main/security/appcues-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Product
- Onboarding
- In-App Guidance
- Analytics
- Customer Success
---
