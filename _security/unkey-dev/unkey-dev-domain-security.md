---
api_specs:
- filename: unkey-dev-openapi.yml
  format: yaml
  label: Unkey Keys API
  slug: unkey-dev-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unkey-dev/refs/heads/main/openapi/unkey-dev-openapi.yml
- filename: unkey-dev-openapi.yml
  format: yaml
  label: Unkey APIs (Namespaces) API
  slug: unkey-dev-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unkey-dev/refs/heads/main/openapi/unkey-dev-openapi.yml
- filename: unkey-dev-openapi.yml
  format: yaml
  label: Unkey Ratelimit API
  slug: unkey-dev-ratelimit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unkey-dev/refs/heads/main/openapi/unkey-dev-openapi.yml
- filename: unkey-dev-openapi.yml
  format: yaml
  label: Unkey Identities API
  slug: unkey-dev-identities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unkey-dev/refs/heads/main/openapi/unkey-dev-openapi.yml
- filename: unkey-dev-openapi.yml
  format: yaml
  label: Unkey Permissions and Roles API
  slug: unkey-dev-permissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unkey-dev/refs/heads/main/openapi/unkey-dev-openapi.yml
- filename: unkey-dev-openapi.yml
  format: yaml
  label: Unkey Analytics API
  slug: unkey-dev-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unkey-dev/refs/heads/main/openapi/unkey-dev-openapi.yml
- filename: unkey-dev-openapi.yml
  format: yaml
  label: Unkey Key Migrations API
  slug: unkey-dev-migrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unkey-dev/refs/heads/main/openapi/unkey-dev-openapi.yml
- filename: unkey-dev-openapi.yml
  format: yaml
  label: Unkey Deploy API
  slug: unkey-dev-deploy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unkey-dev/refs/heads/main/openapi/unkey-dev-openapi.yml
- filename: unkey-dev-openapi.yml
  format: yaml
  label: Unkey Liveness API
  slug: unkey-dev-liveness-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unkey-dev/refs/heads/main/openapi/unkey-dev-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: unkey.com
  spf: true
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: unkey.dev
  spf: true
hosts:
- cert_expires: Sep 11 15:58:00 2026 GMT
  host: www.unkey.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 23:59:59 2026 GMT
  host: api.unkey.com
  hsts: null
  https: true
  tls_version: TLSv1.2
- host: api.unkey.dev
  https: false
kind: domain-security
layout: security
method: probed
name: Unkey Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Unkey, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Unkey
provider_slug: unkey-dev
slug: unkey-dev-domain-security
source_filename: unkey-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.unkey.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 15:58:00 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.unkey.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 30 23:59:59 2026 GMT\n  hsts: null\n- host: api.unkey.dev\n  https: false\ndomains:\n- domain: unkey.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: unkey.dev\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unkey-dev/refs/heads/main/security/unkey-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- API Keys
- Rate Limiting
- Authentication
- Access Control
- Identity
- RBAC
- Analytics
- Open Source
---
