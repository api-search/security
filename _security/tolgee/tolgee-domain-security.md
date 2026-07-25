---
api_specs:
- filename: tolgee-api-keys-api-openapi.yml
  format: yaml
  label: Tolgee API Keys API
  slug: tolgee-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tolgee/refs/heads/main/openapi/tolgee-api-keys-api-openapi.yml
- filename: tolgee-import-export-api-openapi.yml
  format: yaml
  label: Tolgee Import/Export API
  slug: tolgee-import-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tolgee/refs/heads/main/openapi/tolgee-import-export-api-openapi.yml
- filename: tolgee-keys-api-openapi.yml
  format: yaml
  label: Tolgee Keys API
  slug: tolgee-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tolgee/refs/heads/main/openapi/tolgee-keys-api-openapi.yml
- filename: tolgee-languages-api-openapi.yml
  format: yaml
  label: Tolgee Languages API
  slug: tolgee-languages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tolgee/refs/heads/main/openapi/tolgee-languages-api-openapi.yml
- filename: tolgee-projects-api-openapi.yml
  format: yaml
  label: Tolgee Projects API
  slug: tolgee-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tolgee/refs/heads/main/openapi/tolgee-projects-api-openapi.yml
- filename: tolgee-screenshots-api-openapi.yml
  format: yaml
  label: Tolgee Screenshots API
  slug: tolgee-screenshots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tolgee/refs/heads/main/openapi/tolgee-screenshots-api-openapi.yml
- filename: tolgee-translations-api-openapi.yml
  format: yaml
  label: Tolgee Translations API
  slug: tolgee-translations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tolgee/refs/heads/main/openapi/tolgee-translations-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tolgee.io
  spf: true
hosts:
- cert_expires: Aug 11 23:59:59 2026 GMT
  host: tolgee.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 23:43:45 2026 GMT
  host: docs.tolgee.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 13:17:34 2026 GMT
  host: app.tolgee.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tolgee Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tolgee, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Tolgee
provider_slug: tolgee
slug: tolgee-domain-security
source_filename: tolgee-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tolgee.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 11 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.tolgee.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 23:43:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.tolgee.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 13:17:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tolgee.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tolgee/refs/heads/main/security/tolgee-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Localization
- i18n
- Translation
- Open Source
- Developer Tools
---
