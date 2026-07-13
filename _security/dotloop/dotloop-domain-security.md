---
api_specs:
- filename: dotloop-openapi.yml
  format: yaml
  label: dotloop Account API
  slug: dotloop-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dotloop/refs/heads/main/openapi/dotloop-openapi.yml
- filename: dotloop-openapi.yml
  format: yaml
  label: dotloop Profiles API
  slug: dotloop-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dotloop/refs/heads/main/openapi/dotloop-openapi.yml
- filename: dotloop-openapi.yml
  format: yaml
  label: dotloop Loops API
  slug: dotloop-loops-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dotloop/refs/heads/main/openapi/dotloop-openapi.yml
- filename: dotloop-openapi.yml
  format: yaml
  label: dotloop Loop Details API
  slug: dotloop-loop-details-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dotloop/refs/heads/main/openapi/dotloop-openapi.yml
- filename: dotloop-openapi.yml
  format: yaml
  label: dotloop Loop-It API
  slug: dotloop-loop-it-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dotloop/refs/heads/main/openapi/dotloop-openapi.yml
- filename: dotloop-openapi.yml
  format: yaml
  label: dotloop Folders API
  slug: dotloop-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dotloop/refs/heads/main/openapi/dotloop-openapi.yml
- filename: dotloop-openapi.yml
  format: yaml
  label: dotloop Documents API
  slug: dotloop-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dotloop/refs/heads/main/openapi/dotloop-openapi.yml
- filename: dotloop-openapi.yml
  format: yaml
  label: dotloop Participants API
  slug: dotloop-participants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dotloop/refs/heads/main/openapi/dotloop-openapi.yml
- filename: dotloop-openapi.yml
  format: yaml
  label: dotloop Tasks API
  slug: dotloop-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dotloop/refs/heads/main/openapi/dotloop-openapi.yml
- filename: dotloop-openapi.yml
  format: yaml
  label: dotloop Activities API
  slug: dotloop-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dotloop/refs/heads/main/openapi/dotloop-openapi.yml
- filename: dotloop-openapi.yml
  format: yaml
  label: dotloop Contacts API
  slug: dotloop-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dotloop/refs/heads/main/openapi/dotloop-openapi.yml
- filename: dotloop-openapi.yml
  format: yaml
  label: dotloop Loop Templates API
  slug: dotloop-loop-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dotloop/refs/heads/main/openapi/dotloop-openapi.yml
- filename: dotloop-openapi.yml
  format: yaml
  label: dotloop Webhooks API
  slug: dotloop-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dotloop/refs/heads/main/openapi/dotloop-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: dotloop.com
  spf: true
hosts:
- cert_expires: Dec  1 23:59:59 2026 GMT
  host: www.dotloop.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  1 23:59:59 2026 GMT
  host: api-gateway.dotloop.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dotloop Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for dotloop, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: dotloop
provider_slug: dotloop
slug: dotloop-domain-security
source_filename: dotloop-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dotloop.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api-gateway.dotloop.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: dotloop.com\n  dnssec: false\n  caa:\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dotloop/refs/heads/main/security/dotloop-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Real Estate
- Transaction Management
- Loops
- Documents
- E-Signature
- Zillow Group
---
