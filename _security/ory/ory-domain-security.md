---
api_specs:
- filename: ory-api-api-openapi.yml
  format: yaml
  label: Ory api API
  slug: ory-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ory/refs/heads/main/openapi/ory-api-api-openapi.yml
- filename: ory-courier-api-openapi.yml
  format: yaml
  label: Ory courier API
  slug: ory-courier-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ory/refs/heads/main/openapi/ory-courier-api-openapi.yml
- filename: ory-frontend-api-openapi.yml
  format: yaml
  label: Ory frontend API
  slug: ory-frontend-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ory/refs/heads/main/openapi/ory-frontend-api-openapi.yml
- filename: ory-identity-api-openapi.yml
  format: yaml
  label: Ory identity API
  slug: ory-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ory/refs/heads/main/openapi/ory-identity-api-openapi.yml
- filename: ory-jwk-api-openapi.yml
  format: yaml
  label: Ory jwk API
  slug: ory-jwk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ory/refs/heads/main/openapi/ory-jwk-api-openapi.yml
- filename: ory-metadata-api-openapi.yml
  format: yaml
  label: Ory metadata API
  slug: ory-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ory/refs/heads/main/openapi/ory-metadata-api-openapi.yml
- filename: ory-oauth2-api-openapi.yml
  format: yaml
  label: Ory oAuth2 API
  slug: ory-oauth2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ory/refs/heads/main/openapi/ory-oauth2-api-openapi.yml
- filename: ory-oidc-api-openapi.yml
  format: yaml
  label: Ory oidc API
  slug: ory-oidc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ory/refs/heads/main/openapi/ory-oidc-api-openapi.yml
- filename: ory-permission-api-openapi.yml
  format: yaml
  label: Ory permission API
  slug: ory-permission-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ory/refs/heads/main/openapi/ory-permission-api-openapi.yml
- filename: ory-relationship-api-openapi.yml
  format: yaml
  label: Ory relationship API
  slug: ory-relationship-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ory/refs/heads/main/openapi/ory-relationship-api-openapi.yml
- filename: ory-wellknown-api-openapi.yml
  format: yaml
  label: Ory wellknown API
  slug: ory-wellknown-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ory/refs/heads/main/openapi/ory-wellknown-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ory.sh
  spf: true
hosts:
- cert_expires: Sep 23 04:28:42 2026 GMT
  host: www.ory.sh
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ory Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ory, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Ory
provider_slug: ory
slug: ory-domain-security
source_filename: ory-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ory.sh\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 04:28:42 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: ory.sh\n  dnssec: false\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ory/refs/heads/main/security/ory-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Authentication
- Authorization
- Identity
- OAuth2
- OpenID Connect
- Open Source
---
