---
api_specs:
- filename: general-translation-branches-api-openapi.yml
  format: yaml
  label: General Translation Branches API
  slug: general-translation-branches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/general-translation/refs/heads/main/openapi/general-translation-branches-api-openapi.yml
- filename: general-translation-context-api-openapi.yml
  format: yaml
  label: General Translation Context API
  slug: general-translation-context-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/general-translation/refs/heads/main/openapi/general-translation-context-api-openapi.yml
- filename: general-translation-files-api-openapi.yml
  format: yaml
  label: General Translation Files API
  slug: general-translation-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/general-translation/refs/heads/main/openapi/general-translation-files-api-openapi.yml
- filename: general-translation-jobs-api-openapi.yml
  format: yaml
  label: General Translation Jobs API
  slug: general-translation-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/general-translation/refs/heads/main/openapi/general-translation-jobs-api-openapi.yml
- filename: general-translation-project-api-openapi.yml
  format: yaml
  label: General Translation Project API
  slug: general-translation-project-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/general-translation/refs/heads/main/openapi/general-translation-project-api-openapi.yml
- filename: general-translation-tags-api-openapi.yml
  format: yaml
  label: General Translation Tags API
  slug: general-translation-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/general-translation/refs/heads/main/openapi/general-translation-tags-api-openapi.yml
- filename: general-translation-translation-api-openapi.yml
  format: yaml
  label: General Translation Translation API
  slug: general-translation-translation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/general-translation/refs/heads/main/openapi/general-translation-translation-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: gtx.dev
  spf: true
hosts:
- cert_expires: Sep 21 00:12:32 2026 GMT
  host: api2.gtx.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  8 18:55:10 2026 GMT
  host: runtime2.gtx.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: General Translation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for General Translation, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: General Translation
provider_slug: general-translation
slug: general-translation-domain-security
source_filename: general-translation-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api2.gtx.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 00:12:32 2026 GMT\n  hsts: false\n- host: runtime2.gtx.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 18:55:10 2026 GMT\n  hsts: false\ndomains:\n- domain: gtx.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/general-translation/refs/heads/main/security/general-translation-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Internationalization
- Localization
- Translation
- Developer Tools
- Artificial Intelligence
- i18n
- SDKs
- Machine Translation
---
