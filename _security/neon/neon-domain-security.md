---
api_specs:
- filename: neon-auth-webhooks-asyncapi.yml
  format: yaml
  label: Neon Auth
  slug: auth
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/neon/refs/heads/main/asyncapi/neon-auth-webhooks-asyncapi.yml
- filename: neon-api-keys-api-openapi.yml
  format: yaml
  label: Neon API Keys API
  slug: neon-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neon/refs/heads/main/openapi/neon-api-keys-api-openapi.yml
- filename: neon-auth-api-openapi.yml
  format: yaml
  label: Neon Auth API
  slug: neon-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neon/refs/heads/main/openapi/neon-auth-api-openapi.yml
- filename: neon-branches-api-openapi.yml
  format: yaml
  label: Neon Branches API
  slug: neon-branches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neon/refs/heads/main/openapi/neon-branches-api-openapi.yml
- filename: neon-consumption-api-openapi.yml
  format: yaml
  label: Neon Consumption API
  slug: neon-consumption-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neon/refs/heads/main/openapi/neon-consumption-api-openapi.yml
- filename: neon-data-api-api-openapi.yml
  format: yaml
  label: Neon Data API API
  slug: neon-data-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neon/refs/heads/main/openapi/neon-data-api-api-openapi.yml
- filename: neon-databases-api-openapi.yml
  format: yaml
  label: Neon Databases API
  slug: neon-databases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neon/refs/heads/main/openapi/neon-databases-api-openapi.yml
- filename: neon-endpoints-api-openapi.yml
  format: yaml
  label: Neon Endpoints API
  slug: neon-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neon/refs/heads/main/openapi/neon-endpoints-api-openapi.yml
- filename: neon-operations-api-openapi.yml
  format: yaml
  label: Neon Operations API
  slug: neon-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neon/refs/heads/main/openapi/neon-operations-api-openapi.yml
- filename: neon-projects-api-openapi.yml
  format: yaml
  label: Neon Projects API
  slug: neon-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neon/refs/heads/main/openapi/neon-projects-api-openapi.yml
- filename: neon-roles-api-openapi.yml
  format: yaml
  label: Neon Roles API
  slug: neon-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neon/refs/heads/main/openapi/neon-roles-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: neon.com
  spf: true
- caa:
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:sre@neon.tech"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: neon.tech
  spf: true
hosts:
- cert_expires: Sep  3 13:24:42 2026 GMT
  host: neon.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  3 22:49:23 2026 GMT
  host: console.neon.tech
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Neon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Neon, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Neon
provider_slug: neon
slug: neon-domain-security
source_filename: neon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: neon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 13:24:42 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: console.neon.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 22:49:23 2026 GMT\n  hsts: null\ndomains:\n- domain: neon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: neon.tech\n  dnssec: true\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:sre@neon.tech\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/neon/refs/heads/main/security/neon-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Databases
- Serverless
- Postgres
- Infrastructure
- Authentication
- Edge
---
