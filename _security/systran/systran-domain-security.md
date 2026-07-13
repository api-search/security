---
api_specs:
- filename: systran-openapi.yml
  format: yaml
  label: SYSTRAN Translation API
  slug: systran-translation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/systran/refs/heads/main/openapi/systran-openapi.yml
- filename: systran-openapi.yml
  format: yaml
  label: SYSTRAN File Translation API
  slug: systran-file-translation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/systran/refs/heads/main/openapi/systran-openapi.yml
- filename: systran-openapi.yml
  format: yaml
  label: SYSTRAN Supported Languages API
  slug: systran-supported-languages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/systran/refs/heads/main/openapi/systran-openapi.yml
- filename: systran-openapi.yml
  format: yaml
  label: SYSTRAN Language Detection API
  slug: systran-language-detection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/systran/refs/heads/main/openapi/systran-openapi.yml
- filename: systran-openapi.yml
  format: yaml
  label: SYSTRAN NLP API
  slug: systran-nlp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/systran/refs/heads/main/openapi/systran-openapi.yml
- filename: systran-openapi.yml
  format: yaml
  label: SYSTRAN Dictionary API
  slug: systran-dictionary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/systran/refs/heads/main/openapi/systran-openapi.yml
- filename: systran-openapi.yml
  format: yaml
  label: SYSTRAN Profiles API
  slug: systran-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/systran/refs/heads/main/openapi/systran-openapi.yml
- filename: systran-openapi.yml
  format: yaml
  label: SYSTRAN Corpus API
  slug: systran-corpus-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/systran/refs/heads/main/openapi/systran-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: systran.net
  spf: true
hosts:
- cert_expires: Oct  2 03:50:22 2026 GMT
  host: www.systran.net
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 03:50:22 2026 GMT
  host: docs.systran.net
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 03:18:18 2026 GMT
  host: api-translate.systran.net
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Systran Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SYSTRAN, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: SYSTRAN
provider_slug: systran
slug: systran-domain-security
source_filename: systran-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.systran.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 03:50:22 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: docs.systran.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 03:50:22 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api-translate.systran.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 03:18:18 2026 GMT\n  hsts: null\ndomains:\n- domain: systran.net\n  dnssec: true\n  caa:\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/systran/refs/heads/main/security/systran-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Machine Translation
- Translation
- NLP
- Neural Machine Translation
- Localization
- Language Detection
---
