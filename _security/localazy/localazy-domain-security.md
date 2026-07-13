---
api_specs:
- filename: localazy-openapi.yml
  format: yaml
  label: Localazy Import / Upload API
  slug: import-upload
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/localazy/refs/heads/main/openapi/localazy-openapi.yml
- filename: localazy-openapi.yml
  format: yaml
  label: Localazy Export API
  slug: export
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/localazy/refs/heads/main/openapi/localazy-openapi.yml
- filename: localazy-openapi.yml
  format: yaml
  label: Localazy Files API
  slug: files
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/localazy/refs/heads/main/openapi/localazy-openapi.yml
- filename: localazy-openapi.yml
  format: yaml
  label: Localazy Languages API
  slug: languages
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/localazy/refs/heads/main/openapi/localazy-openapi.yml
- filename: localazy-openapi.yml
  format: yaml
  label: Localazy Projects (Management) API
  slug: projects-management
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/localazy/refs/heads/main/openapi/localazy-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: localazy.com
  spf: true
hosts:
- cert_expires: Oct  7 15:42:28 2026 GMT
  host: localazy.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 18 02:04:51 2026 GMT
  host: api.localazy.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Localazy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Localazy, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Localazy
provider_slug: localazy
slug: localazy-domain-security
source_filename: localazy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: localazy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 15:42:28 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: api.localazy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 02:04:51 2026 GMT\n  hsts: null\ndomains:\n- domain: localazy.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/localazy/refs/heads/main/security/localazy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Localization
- Translation
- Internationalization
- i18n
- L10n
- Translation Management
---
