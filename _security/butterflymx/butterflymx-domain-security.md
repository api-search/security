---
api_specs:
- filename: butterflymx-access-groups-api-openapi.yml
  format: yaml
  label: ButterflyMX Access groups API
  slug: butterflymx-access-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/butterflymx/refs/heads/main/openapi/butterflymx-access-groups-api-openapi.yml
- filename: butterflymx-access-logs-api-openapi.yml
  format: yaml
  label: ButterflyMX Access Logs API
  slug: butterflymx-access-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/butterflymx/refs/heads/main/openapi/butterflymx-access-logs-api-openapi.yml
- filename: butterflymx-access-points-api-openapi.yml
  format: yaml
  label: ButterflyMX Access Points API
  slug: butterflymx-access-points-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/butterflymx/refs/heads/main/openapi/butterflymx-access-points-api-openapi.yml
- filename: butterflymx-access-tools-api-openapi.yml
  format: yaml
  label: ButterflyMX Access Tools API
  slug: butterflymx-access-tools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/butterflymx/refs/heads/main/openapi/butterflymx-access-tools-api-openapi.yml
- filename: butterflymx-building-integrations-api-openapi.yml
  format: yaml
  label: ButterflyMX Building Integrations API
  slug: butterflymx-building-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/butterflymx/refs/heads/main/openapi/butterflymx-building-integrations-api-openapi.yml
- filename: butterflymx-buildings-api-openapi.yml
  format: yaml
  label: ButterflyMX Buildings API
  slug: butterflymx-buildings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/butterflymx/refs/heads/main/openapi/butterflymx-buildings-api-openapi.yml
- filename: butterflymx-calls-api-openapi.yml
  format: yaml
  label: ButterflyMX Calls API
  slug: butterflymx-calls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/butterflymx/refs/heads/main/openapi/butterflymx-calls-api-openapi.yml
- filename: butterflymx-devices-api-openapi.yml
  format: yaml
  label: ButterflyMX Devices API
  slug: butterflymx-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/butterflymx/refs/heads/main/openapi/butterflymx-devices-api-openapi.yml
- filename: butterflymx-door-release-requests-api-openapi.yml
  format: yaml
  label: ButterflyMX Door Release Requests API
  slug: butterflymx-door-release-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/butterflymx/refs/heads/main/openapi/butterflymx-door-release-requests-api-openapi.yml
- filename: butterflymx-keychains-api-openapi.yml
  format: yaml
  label: ButterflyMX Keychains API
  slug: butterflymx-keychains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/butterflymx/refs/heads/main/openapi/butterflymx-keychains-api-openapi.yml
- filename: butterflymx-tenant-integrations-api-openapi.yml
  format: yaml
  label: ButterflyMX Tenant Integrations API
  slug: butterflymx-tenant-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/butterflymx/refs/heads/main/openapi/butterflymx-tenant-integrations-api-openapi.yml
- filename: butterflymx-tenants-api-openapi.yml
  format: yaml
  label: ButterflyMX Tenants API
  slug: butterflymx-tenants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/butterflymx/refs/heads/main/openapi/butterflymx-tenants-api-openapi.yml
- filename: butterflymx-units-api-openapi.yml
  format: yaml
  label: ButterflyMX Units API
  slug: butterflymx-units-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/butterflymx/refs/heads/main/openapi/butterflymx-units-api-openapi.yml
- filename: butterflymx-virtual-keys-api-openapi.yml
  format: yaml
  label: ButterflyMX Virtual Keys API
  slug: butterflymx-virtual-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/butterflymx/refs/heads/main/openapi/butterflymx-virtual-keys-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "sectigo.com"
  - 0 iodef "mailto:devops@butterflymx.com"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: butterflymx.com
  spf: true
hosts:
- cert_expires: Sep 25 23:59:59 2026 GMT
  host: butterflymx.com
  hsts: true
  hsts_max_age: 31622400
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 22:07:06 2026 GMT
  host: apidocs.butterflymx.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  3 23:59:59 2026 GMT
  host: api.butterflymx.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Butterflymx Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ButterflyMX, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ButterflyMX
provider_slug: butterflymx
slug: butterflymx-domain-security
source_filename: butterflymx-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: butterflymx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31622400\n- host: apidocs.butterflymx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 22:07:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.butterflymx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  3 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: butterflymx.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"sectigo.com\"\n  - 0 iodef \"mailto:devops@butterflymx.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/butterflymx/refs/heads/main/security/butterflymx-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- access-control
- physical-access
- smart-intercom
- proptech
- property-management
- multifamily
- building-automation
- visitor-management
- iot
- smart-locks
- oauth2
- webhooks
---
