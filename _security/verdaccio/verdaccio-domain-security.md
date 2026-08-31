---
api_specs:
- filename: verdaccio-dist-tags-api-openapi.yml
  format: yaml
  label: Verdaccio dist-tags API
  slug: verdaccio-dist-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/verdaccio/refs/heads/main/openapi/verdaccio-dist-tags-api-openapi.yml
- filename: verdaccio-packages-api-openapi.yml
  format: yaml
  label: Verdaccio packages API
  slug: verdaccio-packages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/verdaccio/refs/heads/main/openapi/verdaccio-packages-api-openapi.yml
- filename: verdaccio-profile-api-openapi.yml
  format: yaml
  label: Verdaccio profile API
  slug: verdaccio-profile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/verdaccio/refs/heads/main/openapi/verdaccio-profile-api-openapi.yml
- filename: verdaccio-publish-api-openapi.yml
  format: yaml
  label: Verdaccio publish API
  slug: verdaccio-publish-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/verdaccio/refs/heads/main/openapi/verdaccio-publish-api-openapi.yml
- filename: verdaccio-search-api-openapi.yml
  format: yaml
  label: Verdaccio search API
  slug: verdaccio-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/verdaccio/refs/heads/main/openapi/verdaccio-search-api-openapi.yml
- filename: verdaccio-tokens-api-openapi.yml
  format: yaml
  label: Verdaccio tokens API
  slug: verdaccio-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/verdaccio/refs/heads/main/openapi/verdaccio-tokens-api-openapi.yml
- filename: verdaccio-user-api-openapi.yml
  format: yaml
  label: Verdaccio user API
  slug: verdaccio-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/verdaccio/refs/heads/main/openapi/verdaccio-user-api-openapi.yml
- filename: verdaccio-utility-api-openapi.yml
  format: yaml
  label: Verdaccio utility API
  slug: verdaccio-utility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/verdaccio/refs/heads/main/openapi/verdaccio-utility-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: verdaccio.org
  spf: true
hosts:
- cert_expires: Sep  3 08:05:21 2026 GMT
  host: www.verdaccio.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Verdaccio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Verdaccio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Verdaccio
provider_slug: verdaccio
slug: verdaccio-domain-security
source_filename: verdaccio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.verdaccio.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 08:05:21 2026 GMT\n  hsts: false\ndomains:\n- domain: verdaccio.org\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/verdaccio/refs/heads/main/security/verdaccio-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- npm
- Registry
- package-manager
- private-registry
- Proxy
- nodejs
- Open-Source
- self-hosted
- yarn
- pnpm
- docker
- kubernetes
---
