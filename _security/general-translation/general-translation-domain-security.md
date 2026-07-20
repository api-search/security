---
api_specs:
- filename: general-translation-openapi-original.yml
  format: yaml
  label: General Translation API
  slug: general-translation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/general-translation/refs/heads/main/openapi/general-translation-openapi-original.yml
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
