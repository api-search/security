---
api_specs:
- filename: simplelocalize-customers-api-openapi.yml
  format: yaml
  label: SimpleLocalize Customers API
  slug: simplelocalize-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simplelocalize/refs/heads/main/openapi/simplelocalize-customers-api-openapi.yml
- filename: simplelocalize-export-api-openapi.yml
  format: yaml
  label: SimpleLocalize Export API
  slug: simplelocalize-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simplelocalize/refs/heads/main/openapi/simplelocalize-export-api-openapi.yml
- filename: simplelocalize-import-api-openapi.yml
  format: yaml
  label: SimpleLocalize Import API
  slug: simplelocalize-import-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simplelocalize/refs/heads/main/openapi/simplelocalize-import-api-openapi.yml
- filename: simplelocalize-languages-api-openapi.yml
  format: yaml
  label: SimpleLocalize Languages API
  slug: simplelocalize-languages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simplelocalize/refs/heads/main/openapi/simplelocalize-languages-api-openapi.yml
- filename: simplelocalize-projects-api-openapi.yml
  format: yaml
  label: SimpleLocalize Projects API
  slug: simplelocalize-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simplelocalize/refs/heads/main/openapi/simplelocalize-projects-api-openapi.yml
- filename: simplelocalize-publication-api-openapi.yml
  format: yaml
  label: SimpleLocalize Publication API
  slug: simplelocalize-publication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simplelocalize/refs/heads/main/openapi/simplelocalize-publication-api-openapi.yml
- filename: simplelocalize-translations-api-openapi.yml
  format: yaml
  label: SimpleLocalize Translations API
  slug: simplelocalize-translations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simplelocalize/refs/heads/main/openapi/simplelocalize-translations-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: simplelocalize.io
  spf: true
hosts:
- cert_expires: Aug 12 06:10:29 2026 GMT
  host: simplelocalize.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 12 06:10:29 2026 GMT
  host: api.simplelocalize.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Simplelocalize Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SimpleLocalize, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: SimpleLocalize
provider_slug: simplelocalize
slug: simplelocalize-domain-security
source_filename: simplelocalize-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: simplelocalize.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 06:10:29 2026 GMT\n  hsts: false\n- host: api.simplelocalize.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 06:10:29 2026 GMT\n  hsts: null\ndomains:\n- domain: simplelocalize.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/simplelocalize/refs/heads/main/security/simplelocalize-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Localization
- Translation
- Internationalization
---
