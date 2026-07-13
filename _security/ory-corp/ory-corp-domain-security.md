---
api_specs:
- filename: ory-corp-openapi.yml
  format: yaml
  label: Ory Identity API (Kratos - Self-Service)
  slug: ory-corp-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ory-corp/refs/heads/main/openapi/ory-corp-openapi.yml
- filename: ory-corp-openapi.yml
  format: yaml
  label: Ory Identity Admin API (Kratos)
  slug: ory-corp-identity-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ory-corp/refs/heads/main/openapi/ory-corp-openapi.yml
- filename: ory-corp-openapi.yml
  format: yaml
  label: Ory OAuth2 and OpenID Connect API (Hydra)
  slug: ory-corp-oauth2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ory-corp/refs/heads/main/openapi/ory-corp-openapi.yml
- filename: ory-corp-openapi.yml
  format: yaml
  label: Ory OAuth2 Admin API (Hydra)
  slug: ory-corp-oauth2-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ory-corp/refs/heads/main/openapi/ory-corp-openapi.yml
- filename: ory-corp-openapi.yml
  format: yaml
  label: Ory Permissions API (Keto)
  slug: ory-corp-permissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ory-corp/refs/heads/main/openapi/ory-corp-openapi.yml
- filename: ory-corp-openapi.yml
  format: yaml
  label: Ory Relationships API (Keto Write)
  slug: ory-corp-relationships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ory-corp/refs/heads/main/openapi/ory-corp-openapi.yml
- filename: ory-corp-openapi.yml
  format: yaml
  label: Ory Courier Messages API
  slug: ory-corp-courier-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ory-corp/refs/heads/main/openapi/ory-corp-openapi.yml
- filename: ory-corp-openapi.yml
  format: yaml
  label: Ory Organizations API (B2B SSO)
  slug: ory-corp-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ory-corp/refs/heads/main/openapi/ory-corp-openapi.yml
- filename: ory-corp-openapi.yml
  format: yaml
  label: Ory Network Projects API (Console)
  slug: ory-corp-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ory-corp/refs/heads/main/openapi/ory-corp-openapi.yml
- filename: ory-corp-openapi.yml
  format: yaml
  label: Ory Network Project API Tokens API
  slug: ory-corp-project-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ory-corp/refs/heads/main/openapi/ory-corp-openapi.yml
- filename: ory-corp-openapi.yml
  format: yaml
  label: Ory Network Event Streams API
  slug: ory-corp-event-streams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ory-corp/refs/heads/main/openapi/ory-corp-openapi.yml
- filename: ory-corp-openapi.yml
  format: yaml
  label: Ory Network Subscriptions and Billing API
  slug: ory-corp-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ory-corp/refs/heads/main/openapi/ory-corp-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ory.com
  spf: true
- caa:
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:security@ory.sh"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ory.sh
  spf: true
hosts:
- cert_expires: Sep 16 20:47:31 2026 GMT
  host: www.ory.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 29 11:16:55 2026 GMT
  host: api.console.ory.sh
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ory Corp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ory, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Ory
provider_slug: ory-corp
slug: ory-corp-domain-security
source_filename: ory-corp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ory.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 20:47:31 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.console.ory.sh\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 11:16:55 2026 GMT\n  hsts: null\ndomains:\n- domain: ory.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: ory.sh\n  dnssec: false\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:security@ory.sh\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ory-corp/refs/heads/main/security/ory-corp-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Identity
- Authentication
- OAuth2
- OpenID Connect
- Authorization
- Permissions
- IAM
- Open Source
---
