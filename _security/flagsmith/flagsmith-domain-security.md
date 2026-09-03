---
api_specs:
- filename: flagsmith-flags-api-openapi.yml
  format: yaml
  label: Flagsmith Flags API
  slug: flags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flagsmith/refs/heads/main/openapi/flagsmith-flags-api-openapi.yml
- filename: flagsmith-environments-api-openapi.yml
  format: yaml
  label: flagsmith Environments API
  slug: flagsmith-environments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flagsmith/refs/heads/main/openapi/flagsmith-environments-api-openapi.yml
- filename: flagsmith-features-api-openapi.yml
  format: yaml
  label: flagsmith Features API
  slug: flagsmith-features-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flagsmith/refs/heads/main/openapi/flagsmith-features-api-openapi.yml
- filename: flagsmith-identities-api-openapi.yml
  format: yaml
  label: flagsmith Identities API
  slug: flagsmith-identities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flagsmith/refs/heads/main/openapi/flagsmith-identities-api-openapi.yml
- filename: flagsmith-organisations-api-openapi.yml
  format: yaml
  label: flagsmith Organisations API
  slug: flagsmith-organisations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flagsmith/refs/heads/main/openapi/flagsmith-organisations-api-openapi.yml
- filename: flagsmith-projects-api-openapi.yml
  format: yaml
  label: flagsmith Projects API
  slug: flagsmith-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flagsmith/refs/heads/main/openapi/flagsmith-projects-api-openapi.yml
- filename: flagsmith-segments-api-openapi.yml
  format: yaml
  label: flagsmith Segments API
  slug: flagsmith-segments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flagsmith/refs/heads/main/openapi/flagsmith-segments-api-openapi.yml
- filename: flagsmith-users-api-openapi.yml
  format: yaml
  label: flagsmith Users API
  slug: flagsmith-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flagsmith/refs/heads/main/openapi/flagsmith-users-api-openapi.yml
- filename: flagsmith-webhooks-api-openapi.yml
  format: yaml
  label: flagsmith Webhooks API
  slug: flagsmith-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flagsmith/refs/heads/main/openapi/flagsmith-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: flagsmith.com
  spf: true
hosts:
- cert_expires: Aug 17 21:35:17 2026 GMT
  host: docs.flagsmith.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 23:59:59 2026 GMT
  host: edge.api.flagsmith.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 19 23:59:59 2026 GMT
  host: api.flagsmith.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Flagsmith Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Flagsmith, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Flagsmith
provider_slug: flagsmith
slug: flagsmith-domain-security
source_filename: flagsmith-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.flagsmith.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 21:35:17 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: edge.api.flagsmith.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 23:59:59 2026 GMT\n  hsts: null\n- host: api.flagsmith.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 19 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: flagsmith.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flagsmith/refs/heads/main/security/flagsmith-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags: []
---
