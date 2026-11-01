---
api_specs:
- filename: roku-apps-api-openapi.yml
  format: yaml
  label: Roku Apps API
  slug: roku-apps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/roku/openapi/roku-apps-api-openapi.yml
- filename: roku-billing-api-openapi.yml
  format: yaml
  label: Roku Billing API
  slug: roku-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/roku/openapi/roku-billing-api-openapi.yml
- filename: roku-builds-api-openapi.yml
  format: yaml
  label: Roku Builds API
  slug: roku-builds-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/roku/openapi/roku-builds-api-openapi.yml
- filename: roku-devices-api-openapi.yml
  format: yaml
  label: Roku Devices API
  slug: roku-devices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/roku/openapi/roku-devices-api-openapi.yml
- filename: roku-diagnostics-api-openapi.yml
  format: yaml
  label: Roku Diagnostics API
  slug: roku-diagnostics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/roku/openapi/roku-diagnostics-api-openapi.yml
- filename: roku-discovery-api-openapi.yml
  format: yaml
  label: Roku Discovery API
  slug: roku-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/roku/openapi/roku-discovery-api-openapi.yml
- filename: roku-groups-api-openapi.yml
  format: yaml
  label: Roku Groups API
  slug: roku-groups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/roku/openapi/roku-groups-api-openapi.yml
- filename: roku-healthz-api-openapi.yml
  format: yaml
  label: Roku Healthz API
  slug: roku-healthz-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/roku/openapi/roku-healthz-api-openapi.yml
- filename: roku-input-api-openapi.yml
  format: yaml
  label: Roku Input API
  slug: roku-input-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/roku/openapi/roku-input-api-openapi.yml
- filename: roku-keypress-api-openapi.yml
  format: yaml
  label: Roku KeyPress API
  slug: roku-keypress-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/roku/openapi/roku-keypress-api-openapi.yml
- filename: roku-organisation-roles-api-openapi.yml
  format: yaml
  label: Roku Organisation Roles API
  slug: roku-organisation-roles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/roku/openapi/roku-organisation-roles-api-openapi.yml
- filename: roku-organisations-api-openapi.yml
  format: yaml
  label: Roku Organisations API
  slug: roku-organisations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/roku/openapi/roku-organisations-api-openapi.yml
- filename: roku-personal-access-tokens-api-openapi.yml
  format: yaml
  label: Roku Personal Access Tokens API
  slug: roku-personal-access-tokens-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/roku/openapi/roku-personal-access-tokens-api-openapi.yml
- filename: roku-projects-api-openapi.yml
  format: yaml
  label: Roku Projects API
  slug: roku-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/roku/openapi/roku-projects-api-openapi.yml
- filename: roku-query-api-openapi.yml
  format: yaml
  label: Roku Query API
  slug: roku-query-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/roku/openapi/roku-query-api-openapi.yml
- filename: roku-snapshots-api-openapi.yml
  format: yaml
  label: Roku Snapshots API
  slug: roku-snapshots-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/roku/openapi/roku-snapshots-api-openapi.yml
- filename: roku-subscription-api-openapi.yml
  format: yaml
  label: Roku Subscription API
  slug: roku-subscription-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/roku/openapi/roku-subscription-api-openapi.yml
- filename: roku-users-api-openapi.yml
  format: yaml
  label: Roku Users API
  slug: roku-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/roku/openapi/roku-users-api-openapi.yml
- filename: roku-validation-api-openapi.yml
  format: yaml
  label: Roku Validation API
  slug: roku-validation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/roku/openapi/roku-validation-api-openapi.yml
- filename: roku-async-api-api-openapi.yml
  format: yaml
  label: Roku Async API
  slug: roku-async-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/roku/openapi/roku-async-api-api-openapi.yml
- filename: roku-service-accounts-api-openapi.yml
  format: yaml
  label: Roku Service Accounts API
  slug: roku-service-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/roku/openapi/roku-service-accounts-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: roku.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: roku.dev
  spf: true
hosts:
- cert_expires: Sep 15 19:27:59 2026 GMT
  host: www.roku.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  9 23:59:59 2026 GMT
  host: developer.roku.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- host: api.cloud.roku.dev
  https: false
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Roku Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Roku, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Roku
provider_slug: roku
slug: roku-domain-security
source_filename: roku-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.roku.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 19:27:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: developer.roku.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.cloud.roku.dev\n  https: false\ndomains:\n- domain: roku.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: roku.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/roku/security/roku-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Streaming
- Television
- Media
- Entertainment
- Connected TV
- Consumer Electronics
---
