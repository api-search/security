---
api_specs:
- filename: ironclad-authorization-api-openapi.yml
  format: yaml
  label: Ironclad Authorization API
  slug: ironclad-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ironclad/refs/heads/main/openapi/ironclad-authorization-api-openapi.yml
- filename: ironclad-entities-api-openapi.yml
  format: yaml
  label: Ironclad Entities API
  slug: ironclad-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ironclad/refs/heads/main/openapi/ironclad-entities-api-openapi.yml
- filename: ironclad-exports-api-openapi.yml
  format: yaml
  label: Ironclad Exports API
  slug: ironclad-exports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ironclad/refs/heads/main/openapi/ironclad-exports-api-openapi.yml
- filename: ironclad-groups-api-openapi.yml
  format: yaml
  label: Ironclad Groups API
  slug: ironclad-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ironclad/refs/heads/main/openapi/ironclad-groups-api-openapi.yml
- filename: ironclad-obligations-api-openapi.yml
  format: yaml
  label: Ironclad Obligations API
  slug: ironclad-obligations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ironclad/refs/heads/main/openapi/ironclad-obligations-api-openapi.yml
- filename: ironclad-records-api-openapi.yml
  format: yaml
  label: Ironclad Records API
  slug: ironclad-records-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ironclad/refs/heads/main/openapi/ironclad-records-api-openapi.yml
- filename: ironclad-resources-api-openapi.yml
  format: yaml
  label: Ironclad Resources API
  slug: ironclad-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ironclad/refs/heads/main/openapi/ironclad-resources-api-openapi.yml
- filename: ironclad-schemas-api-openapi.yml
  format: yaml
  label: Ironclad Schemas API
  slug: ironclad-schemas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ironclad/refs/heads/main/openapi/ironclad-schemas-api-openapi.yml
- filename: ironclad-search-api-openapi.yml
  format: yaml
  label: Ironclad Search API
  slug: ironclad-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ironclad/refs/heads/main/openapi/ironclad-search-api-openapi.yml
- filename: ironclad-users-api-openapi.yml
  format: yaml
  label: Ironclad Users API
  slug: ironclad-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ironclad/refs/heads/main/openapi/ironclad-users-api-openapi.yml
- filename: ironclad-webhooks-api-openapi.yml
  format: yaml
  label: Ironclad Webhooks API
  slug: ironclad-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ironclad/refs/heads/main/openapi/ironclad-webhooks-api-openapi.yml
- filename: ironclad-workflows-api-openapi.yml
  format: yaml
  label: Ironclad Workflows API
  slug: ironclad-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ironclad/refs/heads/main/openapi/ironclad-workflows-api-openapi.yml
description: ''
domains:
- caa:
  - 0 iodef "mailto:security@ironcladhq.com"
  - 0 issue "pki.goog"
  - 0 issue "comodoca.com"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: ironcladapp.com
  spf: true
hosts:
- cert_expires: Aug 22 20:27:09 2026 GMT
  host: developer.ironcladapp.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 19 11:31:57 2026 GMT
  host: na1.ironcladapp.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 14 21:17:12 2026 GMT
  host: clickwrap-developer.ironcladapp.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ironclad Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ironclad, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Ironclad
provider_slug: ironclad
slug: ironclad-domain-security
source_filename: ironclad-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.ironcladapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 20:27:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: na1.ironcladapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 11:31:57 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: clickwrap-developer.ironcladapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 21:17:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ironcladapp.com\n  dnssec: true\n  caa:\n  - 0 iodef \"mailto:security@ironcladhq.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ironclad/refs/heads/main/security/ironclad-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Contract Lifecycle Management
- CLM
- Contracts
- Legal Tech
- LegalOps
- Enterprise
- Workflows
- eSignature
- Clickwrap
- AI
- OAuth
- SCIM
- Webhooks
---
