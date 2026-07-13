---
api_specs:
- filename: openapi.yml
  format: yaml
  label: Yandex Translate API
  slug: yandex-translate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yandex-translate/refs/heads/main/openapi/openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: yandex.cloud
  spf: true
- caa:
  - 0 issue "globalsign.com"
  - 0 issuewild "globalsign.com"
  dmarc: false
  dnssec: false
  domain: yandex.net
  spf: true
hosts:
- cert_expires: Nov 13 20:59:59 2026 GMT
  host: yandex.cloud
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  6 20:59:59 2027 GMT
  host: translate.api.cloud.yandex.net
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Yandex Translate Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Yandex Translate API, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Yandex Translate API
provider_slug: yandex-translate
slug: yandex-translate-domain-security
source_filename: yandex-translate-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: yandex.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 13 20:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: translate.api.cloud.yandex.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 20:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: yandex.cloud\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: yandex.net\n  dnssec: false\n  caa:\n  - 0 issue \"globalsign.com\"\n  - 0 issuewild \"globalsign.com\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yandex-translate/refs/heads/main/security/yandex-translate-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Machine Translation
- Natural Language Processing
- Language Detection
- Translation Dictionary
- Multilingual
- Yandex Cloud
- Localization
- Internationalization
---
